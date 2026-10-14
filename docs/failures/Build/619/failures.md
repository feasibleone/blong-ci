# Failed tests

_feasibleone/blong · workflow Build · build #619_

[Full run](https://github.com/feasibleone/blong/actions/runs/38629534510) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-gogo

- 🔴 failed **src/graceful-shutdown.spawn.test.ts › blong CLI exits 0 with the shutdown marker after timeout sends SIGTERM › exit code 0 (graceful shutdown), got 1** — `src/graceful-shutdown.spawn.test.ts:64`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

