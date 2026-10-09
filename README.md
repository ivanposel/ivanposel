### Ivan Posel — automation & AI systems engineer

I build software that runs unattended — and fixes itself when it breaks. Croatia, working remote on EU time.

**What I'm building**

- **JARVIS** *(private)* — a self-directing platform that runs six social media accounts around the clock: it finds footage, edits it with ffmpeg, captions and safety-checks it with vision models, schedules it through real web apps over the Chrome DevTools Protocol, and proves every step it reports. ~210k lines of Python, 1,370 automated tests, one runtime that replaced 72 separate daemons, and a local 3B model fine-tuned (QLoRA) on its own decisions.
- **An offline AI assistant** *(client product)* — a macOS assistant on a local 14B model for a paying business client. Their data never leaves the machine.

**Libraries pulled out of it** — each one solves a problem JARVIS hit in production:

| | |
|---|---|
| [couldnottell](https://github.com/ivanposel/couldnottell) | A failed measurement is not a value: a three-state UNKNOWN that refuses to be read as zero, plus a linter that finds where code turns failures into numbers. |
| [look-decide-act](https://github.com/ivanposel/look-decide-act) | Drive real web apps over CDP by looking at the page, not by replaying clicks. |
| [leash](https://github.com/ivanposel/leash) | Keep small local LLMs on a leash — look, think, act, verify — so they never act blind. |
| [claimsledger](https://github.com/ivanposel/claimsledger) | Cooperative claims on shared resources, so two background jobs never drive the same browser, GPU or device. |
| [chainwatch](https://github.com/ivanposel/chainwatch) | Ask whether the outcome happened, not whether the process is running. |
| [levers](https://github.com/ivanposel/levers) | One registry owns every kill, restart and reboot, with shared cooldowns and an audit that fails the build on anything else. |
| [damped-camera](https://github.com/ivanposel/damped-camera) | A virtual camera for auto-edited video that moves the way a person would operate it. |

**How I work**

- Fix the cause, not the symptom — find every place the same fault can happen and close them all.
- Prove it, don't assume it — a step is done when the system can show it happened.
- Keep it small — the best code is the code that doesn't need to exist.

**Stack:** Python · Linux / systemd · SQLite · Chrome DevTools Protocol · Playwright · ffmpeg · Ollama · QLoRA · pytest

Open to remote roles — ivanposel@gmail.com
