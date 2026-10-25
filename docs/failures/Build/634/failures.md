# Failed tests

_feasibleone/blong · workflow Build · build #634_

[Full run](https://github.com/feasibleone/blong/actions/runs/40199201955) | [Allure report](index.html)

**8 failing test(s) in 6 package(s)**

## blong-commander

- 🔴 failed **explore.play.ts › kafka-dev — topics and message viewer** — `new`
  - trace: `traces/4ca877a7-360e-4848-9c03-5913b51f9c76-attachment.zip`
- 🔴 failed **explore.play.ts › vault-dev — mounts, secrets, and masked secret viewer** — `new`
  - trace: `traces/fee8f930-254e-4e29-ad5e-1493397a243e-attachment.zip`

## blong-kukum

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the Playwright suite exits 0** — `e2e.test.ts:280`

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
  1..7
  ok 2 - the realm runs its server and browser tests over the added entity # time=17817.959ms
  
  # Subtest: every added primitive is covered by those tests
  ok 1 - all 10 artifacts are covered
  1..1
  ok 3 - every added primitive is covered by those tests # time=0.822ms
  
  # Subtest: the Playwright leg drives the model page against committed baselines
  ok 1 - the added entity has committed baselines
  not ok 2 - the Playwright suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 280
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:280:11)
    source: >2
              }
  ```


## blong-marine

- 🔴 failed **species.play.ts › Marine Species › browse marine species** — `new`
  - trace: `traces/0b9abfbb-9ea7-4e85-b743-f2dbe43a0b5b-attachment.zip`
- 🔴 failed **portal.play.ts › open and close browse tab** — `new`
  - trace: `traces/44f56c15-c018-4e0e-a390-f1a7775093b4-attachment.zip`

## blong-party

- 🔴 failed **unit.play.ts › Party Unit › edit party unit** — `new`
  - trace: `traces/a1250a53-f533-4185-a68a-529dddcfa1f3-attachment.zip`

## blong-sport

- 🔴 failed **index.test.ts › sport flow (server) › sport athlete profile › login › testAdmin permission map includes sportAthleteAdd** — `../../core/blong-chain/executor.ts:444`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  # Subtest: sport flow (server)
  AssertionError [ERR_ASSERTION]: testAdmin permission map includes sportAthleteAdd
  at call (/home/runner/work/blong/blong/core/blong-chain/executor.ts:444:28)
  at Proxy.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:473:44)
  at login (/home/runner/work/blong/blong/realm/blong-sport/server/test/test/testAthlete.ts:51:28)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: sport athlete profile
  # Subtest: login
  not ok 1 - testAdmin permission map includes sportAthleteAdd
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:444:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:473:44)
      login (server/test/test/testAthlete.ts:51:28)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 444
      columnNumber: 28
      functionName: call
  ```


## blong-suite

- 🔴 failed **../../../demo/blong-marine/test/species.play.ts › Marine Species › browse marine species** — `new`
  - trace: `traces/c9161a11-ca11-490a-a1cd-be4c6f48a091-attachment.zip`
