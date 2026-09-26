# Failed tests

_feasibleone/blong · workflow Build · build #583_

[Full run](https://github.com/feasibleone/blong/actions/runs/36269185844) | [Allure report](index.html)

**4 failing test(s) in 3 package(s)**

## blong-cli

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › and nothing was logged to stderr** — `index.test.ts:35`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,12 @@
  -
  +2026-09-26T20:37:54.723Z warn  blong-cli server operation "start adapter" took 2079ms [semlog://t/a6af4ad63a5b]
  +  label: start adapter
  +  elapsedMs: 2079
  +  progress: {"done":1,"total":1}
  +2026-09-26T20:37:56.198Z warn  blong-cli server operation "start text" still running (1470ms) [semlog://t/2f3c0010c151]
  +  label: start text
  +  elapsedMs: 1470
  +  progress: {"done":0,"total":1}
  +2026-09-26T20:37:56.230Z warn  blong-cli server operation "start text" took 1502ms [semlog://t/4389538cf154]
  +  label: start text
  +  elapsedMs: 1502
  +  progress: {"done":1,"total":1}
  ```


## blong-lib

- 🔴 failed **index.test.ts › withProgress › warns when a step finishes past the slow margin › one line: the slow step itself** — `index.test.ts:128`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -1
  +2
  ```

- 🔴 failed **index.test.ts › withProgress › warns when a step finishes past the slow margin › the message reports the elapsed time** — `index.test.ts:136`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/took \d+ms/
  +"operation \"slow step\" still running (11ms)"
  ```


## handler-test-poc

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

