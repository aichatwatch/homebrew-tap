# aichatwatch/homebrew-tap

Homebrew formulae for [AI Chat Watch (AICW)](https://github.com/aichatwatch) projects.

## Install a formula

Install the latest stable release:

```bash
brew install aichatwatch/tap/aicw-video
```

To install the development version from the upstream `main` branch:

```bash
brew install --HEAD aichatwatch/tap/aicw-video
```

Either form pulls Homebrew's `node`, `ffmpeg-full`, and `whisper-cpp` formulae
as dependencies, so you don't need to install them separately.

## Formulae in this tap

| Formula | Description | Source |
| --- | --- | --- |
| [`aicw-video`](Formula/aicw-video.rb) | Local-first video toolkit (CLI + MCP server + web hub for AI-planned shorts). | [aichatwatch/aicw-video](https://github.com/aichatwatch/aicw-video) |

## Updating a formula

After tagging a new upstream release and (if applicable) running
`npm publish`, bump the formula here:

```bash
brew bump-formula-pr \
  --url=https://registry.npmjs.org/aicw-video/-/aicw-video-X.Y.Z.tgz \
  Formula/aicw-video.rb
```

`brew bump-formula-pr` fetches the SHA-256 automatically and opens a PR.

## Maintainer notes

For the full release runbook (npm publish → tag → tap update) see
[aicw-video's release docs](https://github.com/aichatwatch/aicw-video/blob/main/docs/release/HOMEBREW.md).

## Licence

The formulae here are MIT-licensed. Each upstream project has its own
licence — see the project's repository.
