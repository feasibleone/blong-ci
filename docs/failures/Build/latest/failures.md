# Failed tests

_feasibleone/blong · workflow Build · build #609_

[Full run](https://github.com/feasibleone/blong/actions/runs/38297532283) | [Allure report](index.html)

**4 failing test(s) in 3 package(s)**

## blong-gogo

- 🔴 failed **src/frameworkRealms.test.ts › a realm the suite declares is loaded › the declared realm is loaded** — `src/frameworkRealms.test.ts:146`
- 🔴 failed **src/frameworkRealms.test.ts › a trimmed manifest does not un-declare a realm › the file beside the suite still counts** — `src/frameworkRealms.test.ts:166`

## blong-kustomize

- 🔴 failed **index.test.ts › kustomize flow (server) › fill › aBigArchiveIsStreamedRatherThanHeld › the unpack spends 15376 KiB on 16384 KiB of entries** — `server/test/test/testFill.ts:192`

  ```
  simple
  ```


## blong-lib

- 🔴 failed **index.test.ts › withProgress › a step past the margin reports while it runs as well › it says the step is still running** — `index.test.ts:150`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/still running/
  +"operation \"slow step\" took 59ms"
  ```

