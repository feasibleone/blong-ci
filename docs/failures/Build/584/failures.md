# Failed tests

_feasibleone/blong · workflow Build · build #584_

[Full run](https://github.com/feasibleone/blong/actions/runs/36273455630) | [Allure report](index.html)

**3 failing test(s) in 2 package(s)**

## blong-cli

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › and nothing was logged to stderr** — `index.test.ts:48`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,12 @@
  -
  +2026-09-26T21:55:26.533Z warn  blong-cli server operation "start adapter" took 2154ms [semlog://t/a6af4ad63a5b]
  +  label: start adapter
  +  elapsedMs: 2154
  +  progress: {"done":1,"total":1}
  +2026-09-26T21:55:28.300Z warn  blong-cli server operation "start text" still running (1761ms) [semlog://t/2f3c0010c151]
  +  label: start text
  +  elapsedMs: 1761
  +  progress: {"done":0,"total":1}
  +2026-09-26T21:55:28.333Z warn  blong-cli server operation "start text" took 1794ms [semlog://t/4389538cf154]
  +  label: start text
  +  elapsedMs: 1794
  +  progress: {"done":1,"total":1}
  ```


## blong-party

- 🔴 failed **selfRegistration.play.ts › self-registration: create account and auto-login** — `new`
  - trace: `traces/e7686d5c-063b-4b39-953d-3d9d19a2ceb4-attachment.zip`
- 🟡 flaky **profile.play.ts › Party user profile › shows personal details and allows editing the profile and password** — `new`
  - trace: `traces/4c882b02-b12a-4a62-87c4-9d8e0526b870-attachment.zip`
