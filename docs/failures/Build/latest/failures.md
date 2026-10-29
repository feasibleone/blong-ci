# Failed tests

_feasibleone/blong · workflow Build · build #647_

[Full run](https://github.com/feasibleone/blong/actions/runs/40931850744) | [Allure report](index.html)

**5 failing test(s) in 1 package(s)**

## blong-kukum

- 🔴 failed **e2e.test.ts › every added primitive is covered by those tests › ENOENT: no such file or directory, open '/home/runner/work/blong/blong/core/blong-kukum/test/fixture/e2e-realm/meta/dbTest/accessAuthorizationMerge.yaml'** — `e2e.test.ts:78`

  The raw stream around it:

  ```tap
  source: |
  });
  
  t.test(
  --^
      'the realm runs its server and browser tests over the added entity',
      {skip: skipped},
  ...
  
  # Subtest: every added primitive is covered by those tests
  not ok 1 - ENOENT: no such file or directory, open '/home/runner/work/blong/blong/core/blong-kukum/test/fixture/e2e-realm/meta/dbTest/accessAuthorizati…
    ---
    stack: |
      read (e2e.test.ts:78:40)
      Test.t (e2e.test.ts:217:13)
    at:
      fileName: e2e.test.ts
      lineNumber: 78
      columnNumber: 40
      functionName: read
    errno: -2
    code: ENOENT
    syscall: open
  ```

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the Playwright suite exits 0** — `e2e.test.ts:287`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


  The raw stream around it:

  ```tap
  #     at AdapterBase.r…} (http://localhost:5291/s/@fs/home/runner/work/blong/blong/core/blong-browser/src/context/BlongContext.tsx:91)
  # [browser] error: [blong] error dialog gateway.notAllowed Authorization denied: method "e2e.gadget.find" not allowed {type: gateway.notAllowed, messag…
  # [browser] error: Failed to load resource: the server responded with a status of 403 (Forbidden) (http://localhost:5291/rpc/e2e/gadget/find:0)
  # [browser] error: [blong] e2e.gadget.find failed {params: Array(2), error: gateway.notAllowed: Authorization denied: method "e2e.gadget.find" not allo…
  #     at AdapterBase.r…} (http://localhost:5291/s/@fs/home/runner/work/blong/blong/core/blong-browser/src/context/BlongContext.tsx:91)
  # [browser] error: [blong] error dialog gateway.notAllowed Authorization denied: method "e2e.gadget.find" not allowed {type: gateway.notAllowed, messag…
  # [browser] error: Failed to load resource: the server responded with a status of 403 (Forbidden) (http://localhost:5291/rpc/e2e/gadget/find:0)
  # [browser] error: [blong] e2e.gadget.find failed {params: Array(2), error: gateway.notAllowed: Authorization denied: method "e2e.gadget.find" not allo…
  #     at AdapterBase.r…} (http://localhost:5291/s/@fs/home/runner/work/blong/blong/core/blong-browser/src/context/BlongContext.tsx:91)
  # [browser] error: [blong] error dialog gateway.notAllowed Authorization denied: method "e2e.gadget.find" not allowed {type: gateway.notAllowed, messag…
  not ok 2 - the Playwright suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 287
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:287:11)
    source: >2
                  t.comment(`Playwright exited ${status}. Last lines of its output:\n${tail}`);
              }
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added browser group ran** — `e2e.test.ts:196`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,12 @@
  -/e2e flow browser › addGadget$/m
  +String(
  +  # e2e-realm: 9 passed, 2 failed (11 total)
  +  e2e flow (server) › e2e flow › login
  +  e2e flow (server) › e2e flow › addWidget
  +  e2e flow (server) › e2e flow › findWidget
  +  e2e flow (server) › e2e flow › addGadget
  +  e2e flow (server) › e2e flow › findGadget
  +  e2e flow (browser) › e2e flow browser › httpNoAuth
  +  e2e flow (browser) › e2e flow browser › httpAuthDeny
  +  e2e flow (browser) › e2e flow browser › httpAuthPass
  +  e2e flow (browser) › e2e flow browser › login
  +)
  ```


  The raw stream around it:

  ```tap
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -0
      +2
    ...
  
  ok 5 - the added server test ran: add
  ok 6 - the added server test ran: find
  not ok 7 - the added browser group ran
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,12 @@
      -/e2e flow browser › addGadget$/m
      +String(
      +  # e2e-realm: 9 passed, 2 failed (11 total)
      +  e2e flow (server) › e2e flow › login
      +  e2e flow (server) › e2e flow › addWidget
      +  e2e flow (server) › e2e flow › findWidget
      +  e2e flow (server) › e2e flow › addGadget
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the realm suite exits 0** — `e2e.test.ts:179`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


  The raw stream around it:

  ```tap
  ok 2 - regenerated meta/type/gadget.ts
  ok 3 - regenerated server/test/test/testGadget.ts
  ok 4 - regenerated browser/test/test/testGadget.flow.ts
  ok 5 - regenerated meta/model/e2eGadgetModel.ts
  ok 6 - every generated test group was registered
  ok 7 - the committed baselines survived the regeneration
  1..7
  ok 1 - the fixtures are regenerated from the templates on every run # time=72.103ms
  
  # Subtest: the realm runs its server and browser tests over the added entity
  not ok 1 - the realm suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 179
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:179:11)
    source: >2
              }
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the report records no failing test** — `e2e.test.ts:192`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +2
  ```


  The raw stream around it:

  ```tap
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -0
      +1
    ...
  
  ok 2 - no tap failures in the console output
  ok 3 - the tap leg reported into the package (the report holds every runner that did)
  not ok 4 - the report records no failing test
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 192
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:192:11)
    source: >2
                  'the tap leg reported into the package (the report holds every runner that did)',
              );
  ```

