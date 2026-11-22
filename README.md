# Trimlet Endpoint

Call the APIs you use, with their keys kept safe, in a small window driven only by the keyboard.

- Providers (base URL + key) and their endpoints are saved once; variables like `{city}` remember
  their last values.
- The response is shown with colors (JSON, XML); it can be copied, also as a one-line `curl` command
  with `<API_KEY>` in place of the key.
- The keys are kept in the system keychain (Keychain on Mac, Credential Manager on Windows); providers
  and endpoints in the app settings folder (`trimletendpoint/`).

## Build

Written in Go with [Fyne](https://fyne.io), for macOS and Windows. Ready-made downloads are not
published yet. To build it, with Go installed (and on a Mac the Xcode command line tools):

```
go run fyne.io/tools/cmd/fyne@v1.7.3 package --release
```

or `go run .` to try it. The console window comes from [trimlet/gui](https://github.com/trimlet/gui),
which `go` fetches by itself.

## How it is made

The code is written with Claude Opus (Anthropic), under the direction and review of a developer with
almost 30 years of experience. Every feature starts from a real, repeated need, and most ideas are
turned down: the goal is to stay small.

## License

GPL-3.0, see [LICENSE](LICENSE).
