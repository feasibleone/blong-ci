# Failed tests

_feasibleone/blong · workflow Build · build #685_

[Full run](https://github.com/feasibleone/blong/actions/runs/43716302586) | [Allure report](index.html)

**5 failing test(s) in 4 package(s)**

## blong-blob

- 🔴 failed **index.test.ts › blob realm (server) › temp › nothingExpired › Cannot read properties of undefined (reading 'bytes')** — `server/test/test/testTemp.ts:106`

  The raw stream around it:

  ```tap
  label: run test groups
  elapsedMs: 1002
  progress: {"done":5,"total":7}
  2026-11-15T13:25:51.686Z error Watch flow=01M7FP5DEXA9YQE1WMN0BTCPZ9/temp#0 step nothingExpired failed [semlog://r/01M7FP5EE6DC933X3VGA7H9VTJ semlog://t/2a…
  error  TypeError: Cannot read properties of undefined (reading 'bytes')
  TypeError: Cannot read properties of undefined (reading 'bytes')
  at nothingExpired (/home/runner/work/blong/blong/realm/blong-blob/server/test/test/testTemp.ts:106:37)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: nothingExpired
  not ok 1 - Cannot read properties of undefined (reading 'bytes')
    ---
    stack: |
      nothingExpired (server/test/test/testTemp.ts:106:37)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: server/test/test/testTemp.ts
      lineNumber: 106
      columnNumber: 37
      functionName: nothingExpired
    type: TypeError
    tapCaught: returnedPromiseRejection
  ```

- 🔴 failed **index.test.ts › blob realm (server) › temp › sweep › Cannot read properties of undefined (reading 'removed')** — `server/test/test/testTemp.ts:69`

  The raw stream around it:

  ```tap
  ok 1 - expired # time=73.849ms
  
  2026-11-15T13:25:51.625Z error Watch flow=01M7FP5DEXA9YQE1WMN0BTCPZ9/temp#0 step sweep failed [semlog://r/01M7FP5EC9E2E0GA5YWJBJ47VB semlog://t/394afda4792…
  error  TypeError: Cannot read properties of undefined (reading 'removed')
  TypeError: Cannot read properties of undefined (reading 'removed')
  at sweep (/home/runner/work/blong/blong/realm/blong-blob/server/test/test/testTemp.ts:69:34)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: sweep
  not ok 1 - Cannot read properties of undefined (reading 'removed')
    ---
    stack: |
      sweep (server/test/test/testTemp.ts:69:34)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: server/test/test/testTemp.ts
      lineNumber: 69
      columnNumber: 34
      functionName: sweep
    type: TypeError
    tapCaught: returnedPromiseRejection
  ```


## blong-commander

- 🔴 failed **explore.play.ts › s3-dev — buckets and objects** — `new`
  - trace: `traces/c4d5490b-f2a7-4111-acd8-f6b95b83e0ae-attachment.zip`

## blong-int-adapter

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › cleanup › Cannot read properties of undefined (reading 'removed')** — `blob/test/test/testBlobStorageS3.ts:145`

  The raw stream around it:

  ```tap
  ok 5 - missing # time=58.326ms
  
  2026-11-15T13:18:17.147Z error Watch flow=01M7FNQJ1M77WPWZY7BWK9WK8G/blob store on s3#0 step cleanup failed [semlog://r/01M7FNQJHVXCHMB726VVY7AKRM semlog:/…
  error  TypeError: Cannot read properties of undefined (reading 'removed')
  TypeError: Cannot read properties of undefined (reading 'removed')
  at cleanup (/home/runner/work/blong/blong/test/blong-int-adapter/blob/test/test/testBlobStorageS3.ts:145:38)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: cleanup
  not ok 1 - Cannot read properties of undefined (reading 'removed')
    ---
    stack: |
      cleanup (blob/test/test/testBlobStorageS3.ts:145:38)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: blob/test/test/testBlobStorageS3.ts
      lineNumber: 145
      columnNumber: 38
      functionName: cleanup
    type: TypeError
    tapCaught: returnedPromiseRejection
  ```


## blong-sport

- 🟡 flaky **reference.play.ts › Reference › create sport area** — `new`
  - trace: `traces/a57fd7a4-65b6-4699-8720-5cde87bff9d4-attachment.zip`
