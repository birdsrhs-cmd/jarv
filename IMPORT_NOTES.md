# OpenJarvis source import

Upstream: https://github.com/open-jarvis/OpenJarvis

Source snapshot: `103b1227cb65af71fa930de0945e8d11844aef11`.

This import includes patches to restore hidden/minimized desktop windows, honor
backend configuration locations, load only the server CLI during server startup,
and allow speech discovery to be disabled with `[speech] enabled = false`.

Python syntax checks passed. The modified desktop executable has not been built
or verified, and these patches do not yet establish that the black-screen issue
is resolved.

The publication excludes `.github/workflows/` because the publishing credential
does not have workflow scope, and the prebuilt macOS Ollama binary at
`desktop/src-tauri/binaries/ollama-aarch64-apple-darwin` to keep this source import
small. Those files remain in the local upstream clone.

Personal API keys and local runtime configuration are not included.
