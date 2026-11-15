# Failed tests

_feasibleone/blong · workflow Build · build #686_

[Full run](https://github.com/feasibleone/blong/actions/runs/43722139179) | [Allure report](index.html)

**5 failing test(s) in 4 package(s)**

## blong-blob

- 🔴 failed **index.test.ts › blob realm (server) › temp › nothingExpired › and the answer is a count, not a failure — it answered undefined** — `../../core/blong-chain/executor.ts:444`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  2026-11-15T14:29:13.675Z error Watch flow=01M7FSSEF0Y49EXRPDF8Z95NZX/temp#0 step nothingExpired failed [semlog://r/01M7FSSFAB5PJV56GXSZHCPG4C semlog://t/e3…
  error  AssertionError: and the answer is a count, not a failure — it answered undefined
  AssertionError [ERR_ASSERTION]: and the answer is a count, not a failure — it answered undefined
  at call (/home/runner/work/blong/blong/core/blong-chain/executor.ts:444:28)
  at Proxy.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:473:44)
  at nothingExpired (/home/runner/work/blong/blong/realm/blong-blob/server/test/test/testTemp.ts:112:24)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: nothingExpired
  not ok 1 - and the answer is a count, not a failure — it answered undefined
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:444:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:473:44)
      nothingExpired (server/test/test/testTemp.ts:112:24)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 444
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blob realm (server) › temp › sweep › the expired records are gone — the sweep answered undefined** — `../../core/blong-chain/executor.ts:444`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  2026-11-15T14:29:13.596Z error Watch flow=01M7FSSEF0Y49EXRPDF8Z95NZX/temp#0 step sweep failed [semlog://r/01M7FSSF7W9S1YK90Q9XZPPJ4R semlog://t/40910dfa398…
  error  AssertionError: the expired records are gone — the sweep answered undefined
  AssertionError [ERR_ASSERTION]: the expired records are gone — the sweep answered undefined
  at call (/home/runner/work/blong/blong/core/blong-chain/executor.ts:444:28)
  at Proxy.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:473:44)
  at sweep (/home/runner/work/blong/blong/realm/blong-blob/server/test/test/testTemp.ts:72:24)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: sweep
  not ok 1 - the expired records are gone — the sweep answered undefined
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:444:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:473:44)
      sweep (server/test/test/testTemp.ts:72:24)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 444
      columnNumber: 28
      functionName: call
  ```


## blong-commander

- 🔴 failed **explore.play.ts › s3-dev — buckets and objects** — `new`
  - trace: `traces/a2fb540b-1b13-4445-84c3-3f8a96bf9c5e-attachment.zip`

## blong-int-adapter

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › cleanup › the sweep found the expired record — it answered undefined** — `../../core/blong-chain/executor.ts:444`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  2026-11-15T14:22:48.793Z error Watch flow=01M7FSDQ3TJ15E6A9PN5D8938V/blob store on s3#0 step cleanup failed [semlog://r/01M7FSDQESYA8B9927DWA2K6A7 semlog:/…
  error  AssertionError: the sweep found the expired record — it answered undefined
  AssertionError [ERR_ASSERTION]: the sweep found the expired record — it answered undefined
  at call (/home/runner/work/blong/blong/core/blong-chain/executor.ts:444:28)
  at Proxy.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:473:44)
  at cleanup (/home/runner/work/blong/blong/test/blong-int-adapter/blob/test/test/testBlobStorageS3.ts:145:28)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async executeStepFn (/home/runner/work/blong/blong/core/blong-chain/executor.ts:970:34)
  at async Test.<anonymous> (/home/runner/work/blong/blong/core/blong-chain/executor.ts:1134:17)
  # Subtest: cleanup
  not ok 1 - the sweep found the expired record — it answered undefined
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:444:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:473:44)
      cleanup (blob/test/test/testBlobStorageS3.ts:145:28)
      executeStepFn (../../core/blong-chain/executor.ts:970:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1134:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 444
      columnNumber: 28
      functionName: call
  ```


## blong-sport

- 🟡 flaky **deletion.play.ts › Deletion modes › block: a classifier other records point at is refused with the counts** — `new`
  - trace: `traces/21547ff3-2cc2-4196-91f2-c7ead2f6a2e9-attachment.zip`
