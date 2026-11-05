<p align="center">
  <img src="https://raw.githubusercontent.com/tensai-app/.github/main/profile/tensai-mark.png" width="96" alt="tensai">
</p>

<h1 align="center">tensai</h1>

<p align="center">An AI agent that runs on your Android phone. Open models, local tools.<br>Nothing leaves the phone unless you turn it on.</p>

<p align="center"><a href="https://tensai.page">tensai.page</a> · <a href="https://github.com/tensai-app/tensai/releases/latest">Download</a> · <a href="https://tensai.page/docs/">Docs</a> · <a href="https://tensai.page/changelog/">Changelog</a></p>

---

### What it does

- **Runs on the phone.** Any GGUF model, from Hugging Face or a file, through llama.cpp on the CPU or GPU. No server, no account, works offline once a model is downloaded.
- **Fit check.** Each model is rated against your phone's memory before you download it.
- **An agent with guardrails.** Tools for dates, maths, memory, timers, calendar and messages. Anything that sends or deletes shows a confirmation card first.
- **Network is opt-in.** Internet tools stay off until you enable them.

### Repos

| Repo | What |
|---|---|
| [tensai](https://github.com/tensai-app/tensai) | The Android app, Kotlin + Compose |
| [llama.kt](https://github.com/tensai-app/llama.kt) | Kotlin/Android JNI binding for llama.cpp, the engine behind the app |
| [site](https://github.com/tensai-app/site) | Source of [tensai.page](https://tensai.page): landing, docs, changelog |

### Status

Pre-1.0. Latest release is v0.3.6, a signed APK for Android 10+ (arm64-v8a). It works, expect changes between releases.

### License

Apache-2.0.
