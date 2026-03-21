<p align="center"><code>cargo install --path codex-rs/cli --bin forkdex</code></p>
<p align="center"><strong>Forkdex</strong> is a personalized fork of OpenAI Codex CLI with a small set of focused usability improvements on top of upstream.
<p align="center">
  <img src="https://github.com/openai/codex/blob/main/.github/codex-cli-splash.png" alt="Codex CLI splash" width="80%" />
</p>
</br>
Forkdex stays close to upstream Codex, but changes a few daily-use details in the terminal experience.
</br>The upstream project is still available at <a href="https://github.com/openai/codex">openai/codex</a>.</p>

---

## What Forkdex changes

Forkdex is meant to be a practical personal build of Codex rather than a large rewrite. Current improvements include:

- `forkdex` binary defaults and branding instead of `codex`-only wording
- message timestamps in chat history
- preserved timestamps when replaying or resuming sessions
- red highlighting for assistant `but` tokens
- smarter image paste handling, so pasted or dragged local image file paths stay as text while real clipboard image data still attaches as an image

## Relationship To Upstream

This repository is a fork of [openai/codex](https://github.com/openai/codex) and keeps the upstream structure, docs, and build system wherever possible.

Most of the documentation below still refers to `codex`, OpenAI's original naming, and upstream distribution paths. In this fork, the customized CLI binary is `forkdex`.

## Quickstart

### Installing and running Forkdex

Build the customized CLI from source:

```shell
cargo install --path codex-rs/cli --bin forkdex
```

Then run `forkdex` to get started.

If you want the upstream distribution instead, follow the original Codex instructions below.

<details>
<summary>You can also go to the <a href="https://github.com/openai/codex/releases/latest">latest GitHub Release</a> and download the appropriate binary for your platform.</summary>

Each GitHub Release contains many executables, but in practice, you likely want one of these:

- macOS
  - Apple Silicon/arm64: `codex-aarch64-apple-darwin.tar.gz`
  - x86_64 (older Mac hardware): `codex-x86_64-apple-darwin.tar.gz`
- Linux
  - x86_64: `codex-x86_64-unknown-linux-musl.tar.gz`
  - arm64: `codex-aarch64-unknown-linux-musl.tar.gz`

Each archive contains a single entry with the platform baked into the name (e.g., `codex-x86_64-unknown-linux-musl`), so you likely want to rename it to `codex` after extracting it.

</details>

### Using Codex with your ChatGPT plan

Run `codex` and select **Sign in with ChatGPT**. We recommend signing into your ChatGPT account to use Codex as part of your Plus, Pro, Team, Edu, or Enterprise plan. [Learn more about what's included in your ChatGPT plan](https://help.openai.com/en/articles/11369540-codex-in-chatgpt).

You can also use Codex with an API key, but this requires [additional setup](https://developers.openai.com/codex/auth#sign-in-with-an-api-key).

## Docs

- [**Codex Documentation**](https://developers.openai.com/codex)
- [**Contributing**](./docs/contributing.md)
- [**Installing & building**](./docs/install.md)
- [**Open source fund**](./docs/open-source-fund.md)

This repository is licensed under the [Apache-2.0 License](LICENSE).
