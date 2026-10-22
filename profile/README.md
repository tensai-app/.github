<p align="center">
  <img src="https://raw.githubusercontent.com/tensai-app/.github/main/profile/tensai-mark.png" width="96" alt="tensai">
</p>

<h1 align="center">tensai</h1>

<p align="center">On-device AI for Android. Local models, local tools.<br>Nothing leaves the phone unless you turn it on.</p>

<p align="center"><a href="https://tensai.page">tensai.page</a> · <a href="https://tensai.page/docs/">Docs</a> · <a href="https://tensai.page/changelog/">Changelog</a></p>

---

| Repo | What |
|---|---|
| tensai (private until v1.0) | The Android app: chat with GGUF models, tools and phone actions, all on the phone |
| [llama.kt](https://github.com/tensai-app/llama.kt) | Kotlin/Android JNI binding for llama.cpp, the engine behind tensai |

### How it works

- **Runs on the phone.** llama.cpp on the CPU (or Vulkan when it is faster), no server, no account.
- **Tools, not a toy.** Timers, calendar, drafts, memory, web search: the model acts through your apps, and you confirm.
- **Network is opt-in.** Off by default. When on, every request shows where it went and what was sent.
- **Measured, not guessed.** Perf work comes with numbers from a real mid-range phone (Dimensity 900, 8 GB).

### Status

Working releases (v0.3.x) ship as signed APKs. The public v1.0 is next.
