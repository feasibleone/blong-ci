# Failed tests

_feasibleone/blong · workflow Build · build #555_

[Full run](https://github.com/feasibleone/blong/actions/runs/34963948624) | [Allure report](index.html)

**5 failing test(s) in 3 package(s)**

## blong-kukum

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added browser group ran** — `e2e.test.ts:153`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,5 @@
  -/\bok \d+ - e2e flow browser\b/
  +String(
  +  # e2e-realm: 0 passed, 0 failed (0 total)
  +  # raw report: .ci-report/tap.json, structured: .ci-report/report.json
  +  
  +)
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: add** — `e2e.test.ts:151`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,5 @@
  -/\bok \d+ - addGadget\b/
  +String(
  +  # e2e-realm: 0 passed, 0 failed (0 total)
  +  # raw report: .ci-report/tap.json, structured: .ci-report/report.json
  +  
  +)
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: find** — `e2e.test.ts:152`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,5 @@
  -/\bok \d+ - findGadget\b/
  +String(
  +  # e2e-realm: 0 passed, 0 failed (0 total)
  +  # raw report: .ci-report/tap.json, structured: .ci-report/report.json
  +  
  +)
  ```


## semantic-log

- 🔴 failed **(unparsed) › tap reported 2 failure(s) absent from its JSON report**

## blong-access

- 🟡 flaky **role.play.ts › Access Role › cleanup access role**
  - trace: `traces/58fba839-1393-4a5d-ba49-bdabb93ee416-attachment.zip`
