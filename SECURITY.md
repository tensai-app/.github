# Security policy

## Reporting a vulnerability

Report privately. Do not open a public issue.

1. Go to the Security tab of the affected repo and use "Report a vulnerability" ([tensai](https://github.com/tensai-app/tensai/security/advisories/new), [llama.kt](https://github.com/tensai-app/llama.kt/security/advisories/new), [site](https://github.com/tensai-app/site/security/advisories/new)). This opens a private GitHub security advisory that only you and the maintainer see.
2. If you can't use that, write to security@tensai.page (the contact in the site's [security.txt](https://tensai.page/.well-known/security.txt)).

Include what you can: version of the app, device and Android version, steps to reproduce, impact. A proof of concept helps, a crash log helps.

## Scope

In scope:

- the tensai app: tool confirmation bypass, data leaving the phone without the user turning a network tool on, prompt or chat content reaching logs, permission misuse, anything that makes the app act without the confirmation card it should show;
- llama.kt: memory safety bugs in the JNI layer or the patches carried on llama.cpp, template or tokenization issues that let message text forge turns;
- the site: XSS, CSP bypass, anything that serves third-party content.

Out of scope: vulnerabilities in upstream llama.cpp or a model itself with no tensai-specific angle (report those upstream), a model saying something wrong or unsafe, issues that need a rooted or already-compromised phone.

## What to expect

One maintainer, no SLA. Reports are read as they come. A fix ships in the next release and is credited in the advisory unless you prefer otherwise. Please give time to ship a fix before you publish.

## Supported versions

Pre-1.0: only the latest release gets fixes.
