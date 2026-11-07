# Contributing to tensai

tensai is an Android app that runs a local AI agent on the phone, on top of llama.cpp. Pre-1.0, one maintainer, one test phone. This file is the entry point for the whole org: it applies to every repo that has no CONTRIBUTING.md of its own.

## The most useful thing you can do: run it on your phone

One test device (Dimensity 900, Mali-G68, 8 GB) cannot tell what the app does on a Snapdragon, an Exynos, a Tensor or a 12 GB phone. The fit rating and the default backend are calibrated on that single device. Every phone that runs the app and reports numbers widens what can be measured and fixed: SoC, GPU, RAM, Android version.

No code needed, under 10 minutes once the model is downloaded:

1. Install the APK from [GitHub Releases](https://github.com/tensai-app/tensai/releases/latest). arm64-v8a, Android 10 or later.
2. Load a model (download one from inside the app, or import a GGUF).
3. Settings > This device > Benchmark > Run the benchmark. It takes about 2 to 5 minutes, you can stop it, and the phone may warm up. Tap Copy when it ends.
4. Open a [Device report](https://github.com/tensai-app/tensai/issues/new?template=device_report.yml) and paste.

The app sends nothing. The benchmark runs on the model already loaded, with no tools and no network, and the result stays on screen until you copy it. Only what you paste into the issue is shared, and the report holds no conversation content: app version, phone model, SoC, RAM, Android version, model name, quant, backend, threads, speeds, charging and thermal state. Read it before you post, it is plain text.

The Benchmark card is not in v0.3.6. It ships in the release after it. Until then, build from source ([tensai/CONTRIBUTING.md](https://github.com/tensai-app/tensai/blob/main/CONTRIBUTING.md)) or report numbers by hand in a bug report.

Other ways to help without code:

- Ask for a model that does not load or is rated wrong: [Model request](https://github.com/tensai-app/tensai/issues/new?template=model_request.yml).
- Report a bug: [Bug report](https://github.com/tensai-app/tensai/issues/new?template=bug_report.yml).
- Fix a typo or a wrong sentence in the docs (see the site repo below).

## Where things go

| You want to | Repo |
|---|---|
| Report a bug or a device result, request a model, change the app | [tensai](https://github.com/tensai-app/tensai) |
| Change inference, the llama.cpp patches, the JNI binding, a native crash | [llama.kt](https://github.com/tensai-app/llama.kt) |
| Fix the landing page, the docs or the changelog page | [site](https://github.com/tensai-app/site) |

Not sure which one: open the issue in `tensai`, it gets moved if needed. Each repo's CONTRIBUTING.md has the build steps, the checks to run before a PR and the commit rules.

## Issues

- Search first, a device report for your phone may already exist: add yours anyway, a second measurement on the same SoC is still data.
- One problem per issue.
- Never paste conversations, memory content, API keys or tokens. Logs: trim them to the relevant lines.
- Security problems do not go in issues, see [SECURITY.md](SECURITY.md).

Labels: `device-report`, `model-request`, `bug`, `good first issue`.

## Pull requests

- Small and focused beats big. For anything larger than a fix, open an issue first so we agree on the direction before you write it.
- Fork, branch from `main`, open the PR against `main`. CI runs on every PR.
- Commits and PR titles follow Conventional Commits: `type(scope): subject`. Types: feat, fix, perf, refactor, docs, test, build, ci, chore, revert, style.
- Don't cite issue numbers in commit subjects. Link the issue in the PR description.
- Run the checks of the repo you touched and say in the PR what you ran. A change that touches native code or the UI says on which device it was tested.

## License

Apache-2.0. By sending a contribution you agree it is released under the license of the repo it goes to.
