# Failed tests

_feasibleone/blong · workflow Build · build #705_

[Full run](https://github.com/feasibleone/blong/actions/runs/44913958551) | [Allure report](index.html)

**58 failing test(s) in 10 package(s)**

## blong-blob

- 🔴 failed **index.test.ts › blob realm (server)** — `index.test.ts:25`

  The raw stream around it:

  ```tap
      2026-11-21T14:50:25.514Z info  blob.store event adapter.stop [lukaot://t/0cc3bf136c8a p=01M7Z9CKBA7DTS5423C7HETHQQ]
        portType: dispatch
      2026-11-21T14:50:25.514Z info  blob.blobDispatch event adapter.stop [lukaot://t/0cc3bf136c8a p=01M7Z9CKBA7DTS5423C7HETHQR]
        portType: dispatch
      2026-11-21T14:50:25.514Z info  blob.testDispatch event adapter.stop [lukaot://t/0cc3bf136c8a p=01M7Z9CKBA7DTS5423C7HETHQS]
        portType: dispatch
      2026-11-21T14:50:25.514Z info  testRealm.testDispatch event adapter.stop [lukaot://t/0cc3bf136c8a p=01M7Z9CKBA7DTS5423C7HETHQT]
        portType: dispatch
      1..3
      # time=6286.354ms
  not ok 5 - index.test.ts # time=6286.354ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-blob
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.3/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_/…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-blob/index.test.ts
    jobId: 1
  ```

- 🔴 failed **index.test.ts › blob realm (server) › blob: content does not match its digest (eac6806ffea41e357eff65e138aa32869931759a787f2f6eed7f1bb2419f293f ≠ a99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99f)** — `store/storageDigest.ts:78`

  The raw stream around it:

  ```tap
      isToplevel: true
    source: >2
          const context = test || (await import('node:test')).default;
          return steps =>
              context.test(
      ----------------^
                  steps.name,
                  runSteps(steps, log, options) as (t: unknown) => void | Promise<void>,
    ...
  
  not ok 8 - blob: content does not match its digest (eac6806ffea41e357eff65e138aa32869931759a787f2f6eed7f1bb2419f293f ≠ a99fa99fa99fa99fa99fa99fa99fa99f…
    ---
    stack: |
      Transform.flush (store/storageDigest.ts:78:21)
    at:
      fileName: store/storageDigest.ts
      lineNumber: 78
      columnNumber: 21
      typeName: Transform
      methodName: flush
      functionName: Transform.flush
    type: blob.corrupt
    expected: a99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99fa99f
  ```

- 🔴 failed **index.test.ts › blob realm (server) › crypto › aRecordWhoseDigestIsWrongIsRefused › a digest that does not match the plaintext is a refusal, not a wrong file** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  ...
  
  # Subtest: twoEqualFilesAreEncryptedDifferently
  1..0
  ok 3 - twoEqualFilesAreEncryptedDifferently # time=37.046ms
  
  2026-11-21T14:50:24.693Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRecordWhoseDigestIsWrongIsRefused failed: a digest t…
  step: aRecordWhoseDigestIsWrongIsRefused
  reason: a digest that does not match the plaintext is a refusal, not a wrong file
  # Subtest: aRecordWhoseDigestIsWrongIsRefused
  not ok 1 - a digest that does not match the plaintext is a refusal, not a wrong file
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      aRecordWhoseDigestIsWrongIsRefused (server/test/test/testCrypto.ts:171:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blob realm (server) › crypto › aRoundTripAnswersThePlaintext › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testCrypto.ts:12`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › crypto › theStoredBytesAreNotThePlaintext › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testCrypto.ts:12`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › read › aNamedDownloadIsAnswered › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testRead.ts:19`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › read › theAnswerCarriesWhatABrowserNeeds › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testRead.ts:19`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › upload › aCommittedBlobHasNoLifetime › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testUpload.ts:25`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › upload › aFileArrivesInThreeSteps › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testUpload.ts:25`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › upload › aStoredKeyIsNotWrittenTwice › Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')** — `server/test/test/testUpload.ts:25`

  The raw stream around it:

  ```tap
  ok 4 - missingBlobAnswersNull # time=3.371ms
  
  1..4
  ok 1 - storage # time=152.419ms
  
  2026-11-21T14:50:24.597Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBMS/crypto#0 intent=test.crypto step aRoundTripAnswersThePlaintext failed: Cannot read pro…
  step: aRoundTripAnswersThePlaintext
  reason: Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
  # Subtest: crypto
  # Subtest: aRoundTripAnswersThePlaintext
  not ok 1 - Cannot read properties of undefined (reading 'Symbol(Symbol.asyncIterator)')
    ---
    stack: |
      readAll (server/test/test/testCrypto.ts:12:31)
      aRoundTripAnswersThePlaintext (server/test/test/testCrypto.ts:58:40)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testCrypto.ts
      lineNumber: 12
      columnNumber: 31
      functionName: readAll
    type: TypeError
  ```

- 🔴 failed **index.test.ts › blob realm (server) › variants › theThumbRouteAnswersTheDerivedSize › the thumbnail serves as a variant of the same key** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  ok 3 - nothingExpired # time=22.643ms
  
  1..3
  ok 6 - temp # time=137.715ms
  
  2026-11-21T14:50:25.407Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBN3/variants#0 intent=test.variants step thumbnail failed: the thumbnail serves as a varia…
  step: thumbnail
  reason: the thumbnail serves as a variant of the same key
  # Subtest: variants
  # Subtest: thumbnail
  not ok 1 - the thumbnail serves as a variant of the same key
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      thumbnail (server/test/test/testVariants.ts:90:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blob realm (server) › variants › thumbnail › the thumbnail serves as a variant of the same key** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  ok 3 - nothingExpired # time=22.643ms
  
  1..3
  ok 6 - temp # time=137.715ms
  
  2026-11-21T14:50:25.407Z error Watch flow=01M7Z9CJ8NJ716J3QJJW25KBN3/variants#0 intent=test.variants step thumbnail failed: the thumbnail serves as a varia…
  step: thumbnail
  reason: the thumbnail serves as a variant of the same key
  # Subtest: variants
  # Subtest: thumbnail
  not ok 1 - the thumbnail serves as a variant of the same key
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      thumbnail (server/test/test/testVariants.ts:90:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```


## blong-commander

- 🔴 failed **observedBranchList.play.ts › the orchestrator dispatch is drawn with its milestones and its outgoing leg** — `new`
  - trace: `traces/1c03fbf7-d321-41e9-ab27-24a9cb92737c-attachment.zip`

## blong-gateway

- 🔴 failed **observedMergeFlow.play.ts › a checkpoint and a branch are drawn for a flow this realm served** — `new`
  - trace: `traces/67287344-4d11-485e-9670-fb7a673ff850-attachment.zip`
- 🔴 failed **observedFlow.play.ts › a flow this realm served is drawn as a diagram** — `new`
  - trace: `traces/ba77390c-fe84-474b-9846-330e31ec8677-attachment.zip`
- 🔴 failed **observedMergeFlow.play.ts › the branch the handler took is drawn as an alt block** — `new`
  - trace: `traces/117f77c2-bf34-4760-a304-ae99f9761da4-attachment.zip`

## blong-int-adapter

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › missing › the blob reads back** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  # Subtest: blong int-adapter
  # Subtest: blob store on s3
  # Subtest: upload
  1..0
  ok 1 - upload # time=172.82ms
  
  2026-11-21T14:43:48.881Z error Watch flow=01M7Z90FQMNCQF3ZHH31KRZXA4/blob store on s3#0 intent=test.blobStorageS3 step read failed: the blob reads back [lu…
  step: read
  reason: the blob reads back
  # Subtest: read
  not ok 1 - the blob reads back
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      read (blob/test/test/testBlobStorageS3.ts:76:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › read › the blob reads back** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  # Subtest: blong int-adapter
  # Subtest: blob store on s3
  # Subtest: upload
  1..0
  ok 1 - upload # time=172.82ms
  
  2026-11-21T14:43:48.881Z error Watch flow=01M7Z90FQMNCQF3ZHH31KRZXA4/blob store on s3#0 intent=test.blobStorageS3 step read failed: the blob reads back [lu…
  step: read
  reason: the blob reads back
  # Subtest: read
  not ok 1 - the blob reads back
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      read (blob/test/test/testBlobStorageS3.ts:76:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › record › the blob reads back** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  # Subtest: blong int-adapter
  # Subtest: blob store on s3
  # Subtest: upload
  1..0
  ok 1 - upload # time=172.82ms
  
  2026-11-21T14:43:48.881Z error Watch flow=01M7Z90FQMNCQF3ZHH31KRZXA4/blob store on s3#0 intent=test.blobStorageS3 step read failed: the blob reads back [lu…
  step: read
  reason: the blob reads back
  # Subtest: read
  not ok 1 - the blob reads back
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      read (blob/test/test/testBlobStorageS3.ts:76:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **blob.test.ts › blong int-adapter › blob store on s3 › remove › the blob reads back** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  # Subtest: blong int-adapter
  # Subtest: blob store on s3
  # Subtest: upload
  1..0
  ok 1 - upload # time=172.82ms
  
  2026-11-21T14:43:48.881Z error Watch flow=01M7Z90FQMNCQF3ZHH31KRZXA4/blob store on s3#0 intent=test.blobStorageS3 step read failed: the blob reads back [lu…
  step: read
  reason: the blob reads back
  # Subtest: read
  not ok 1 - the blob reads back
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      read (blob/test/test/testBlobStorageS3.ts:76:28)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **http.test.ts › blong int-adapter › http echo GET › echoRequest › Echo should return a response** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  2026-11-21T14:43:47.737Z info  Server listening at http://127.0.0.1:36327 [lukaot://t/66dfd34d2658 p=01M7Z90ET2R46X626YZVFY1PC7]
  2026-11-21T14:43:47.737Z info  Server listening at http://10.1.0.241:36327 [lukaot://t/66dfd34d2658 p=01M7Z90EWSFXWVBF2D0PTC5RRT]
  2026-11-21T14:43:47.738Z info  Server listening at http://172.18.0.1:36327 [lukaot://t/66dfd34d2658 p=01M7Z90EWSFXWVBF2D0PTC5RRV]
  2026-11-21T14:43:47.738Z warn  gateway gateway listening at random port 36327 [lukaot://t/9d26c0d66b06 p=01M7Z90EWT18AM9PWMT6HN2TYQ]
  2026-11-21T14:43:47.911Z error Watch flow=01M7Z90EXYT3131WFH2PEXEAPS/http echo GET#0 intent=test.http.echoGet step echoRequest failed: Echo should return a…
  step: echoRequest
  reason: Echo should return a response
  # Subtest: blong int-adapter
  # Subtest: http echo GET
  # Subtest: echoRequest
  not ok 1 - Echo should return a response
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      echoRequest (http/test/test/testHttpEchoGet.ts:12:24)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```


## blong-log

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › AllFiltersShowcase › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 3.0150945216049383% different from snapshot (62521 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--all-filters-showcase-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › DarkTheme › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 3.0150945216049383% different from snapshot (62521 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--dark-theme-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › Empty › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.08116319444444445% different from snapshot (1683 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--empty-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ErrorsOnly › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.9228395061728395% different from snapshot (19136 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--errors-only-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedExceptionDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.0541570216049383% different from snapshot (21859 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-exception-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedHTTPDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.2351466049382718% different from snapshot (25612 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-http-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedMixedContent › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.9603587962962963% different from snapshot (19914 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-mixed-content-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › FilteredServer › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 3.155140817901234% different from snapshot (65425 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--filtered-server-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPErrorWithBody › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.6509934413580246% different from snapshot (13499 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-error-with-body-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPFullDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.2332175925925926% different from snapshot (25572 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-full-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPSuccessWithBody › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.6633873456790124% different from snapshot (13756 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-success-with-body-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPWithCacheHeaders › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.5964506172839507% different from snapshot (12368 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-with-cache-headers-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LargeDataset › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 7.820457175925926% different from snapshot (162165 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--large-dataset-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
      at runNextTicks (node:internal/process/task_queues:65:5)
      at processImmediate (node:internal/timers:541:9)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LargeDatasetLight › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 7.906201774691358% different from snapshot (163943 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--large-dataset-light-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LightTheme › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 3.044656635802469% different from snapshot (63134 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--light-theme-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotCapturesExpanded › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.373070987654321% different from snapshot (28472 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-captures-expanded-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotFrameDump › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.7496624228395062% different from snapshot (15545 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-frame-dump-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotFrameDumpLight › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.755787037037037% different from snapshot (15672 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-frame-dump-light-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotRecordContext › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.7107928240740741% different from snapshot (14739 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-record-context-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotRecords › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 2.462818287037037% different from snapshot (51069 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-records-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LukaotSignalExpanded › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.1645447530864197% different from snapshot (24148 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--lukaot-signal-expanded-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingExpanded › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.7113233024691359% different from snapshot (14750 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-expanded-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingHTTPAndErrors › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.0794753086419753% different from snapshot (22384 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-http-and-errors-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingSingleLine › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.4139178240740741% different from snapshot (8583 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-single-line-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SingleService › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.6369116512345679% different from snapshot (13207 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--single-service-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SingleTrace › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.056712962962963% different from snapshot (21912 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--single-trace-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › WithHTTPDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 1.5266685956790123% different from snapshot (31657 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--with-http-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:196:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › tools/blong-log/src/client/LogViewer.stories.tsx — test file failed to run** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
    ● LogViewer › DarkTheme › smoke-test
  
      Expected image to match or be a close match to snapshot but was 3.0150945216049383% different from snapshot (62521 differing pixels).
      See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--dark-theme-diff.png
  
        194 |             // Full-page screenshot comparison — saves real PNG files
        195 |             const screenshot = await page.screenshot({fullPage: true});
      > 196 |             expect(screenshot).toMatchImageSnapshot({
            |                                ^
        197 |                 customSnapshotsDir: path.join(
        198 |                     __dirname,
        199 |                     '..',
  
        at postVisit (tools/blong-log/.storybook/test-runner.cjs:196:32)
  
    ● LogViewer › LightTheme › smoke-test
  
      Expected image to match or be a close match to snapshot but was 3.044656635802469% different from snapshot (63134 differing pixels).
      See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--light-theme-diff.png
  
        194 |             // Full-page screenshot com
  ```


## blong-party

- 🔴 failed **profile.play.ts › Party user profile › stores a photograph and shows it on the avatar** — `new`
  - trace: `traces/d93f6d99-ce40-4910-af42-a9f2c57c4af0-attachment.zip`

## blong-realm

- 🔴 failed **index.test.ts › blong flow (server) › blong realm flow › findFlows › the unions of every observed kind** — `../blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  2026-11-21T14:35:43.142Z warn  registry operation "ready ports" took 3095ms [lukaot://t/0a359aa315dd p=01M7Z8HNN6TNMA1R22BR8MWGFC]
  label: ready ports
  elapsedMs: 3095
  progress: {"done":6,"total":6}
  2026-11-21T14:35:43.345Z error Watch flow=01M7Z8HNQWC6Z9F7B4YG37GK4D/blong realm flow#0 intent=test.blongRealmFlow step findFlows failed: the unions of eve…
  step: findFlows
  reason: the unions of every observed kind
  # Subtest: blong flow (server)
  # Subtest: blong realm flow
  # Subtest: findFlows
  not ok 1 - the unions of every observed kind
    ---
    stack: |
      call (../blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../blong-chain/executor.ts:498:44)
      findFlows (server/test/test/testBlongRealmFlow.ts:33:28)
      executeStepFn (../blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../blong-chain/executor.ts:1174:17)
    at:
      fileName: ../blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blong flow (server) › blong realm flow › findTemplates › the templates the run has taught the service** — `../blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
              await scope.test(name, async (sub: unknown) => {
  ------------------------^
                  started = true;
                  await run(sub as ITestFrameworkContext);
  ...
  
  2026-11-21T14:35:43.386Z error Watch flow=01M7Z8HNQWC6Z9F7B4YG37GK4D/blong realm flow#0 intent=test.blongRealmFlow step findTemplates failed: the templates…
  step: findTemplates
  reason: the templates the run has taught the service
  # Subtest: findTemplates
  not ok 1 - the templates the run has taught the service
    ---
    stack: |
      call (../blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../blong-chain/executor.ts:498:44)
      findTemplates (server/test/test/testBlongRealmFlow.ts:44:28)
      executeStepFn (../blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../blong-chain/executor.ts:1174:17)
    at:
      fileName: ../blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blong flow (server) › blong realm flow › getDigest › the stream answers** — `../blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
              await scope.test(name, async (sub: unknown) => {
  ------------------------^
                  started = true;
                  await run(sub as ITestFrameworkContext);
  ...
  
  2026-11-21T14:35:43.407Z error Watch flow=01M7Z8HNQWC6Z9F7B4YG37GK4D/blong realm flow#0 intent=test.blongRealmFlow step getDigest failed: the stream answer…
  step: getDigest
  reason: the stream answers
  # Subtest: getDigest
  not ok 1 - the stream answers
    ---
    stack: |
      call (../blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../blong-chain/executor.ts:498:44)
      getDigest (server/test/test/testBlongRealmFlow.ts:57:28)
      executeStepFn (../blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../blong-chain/executor.ts:1174:17)
    at:
      fileName: ../blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```

- 🔴 failed **index.test.ts › blong flow (server) › blong realm flow › getUnknownFlow › Missing expected rejection: an execution the service never retained is refused rather than drawn empty** — `server/test/test/testBlongRealmFlow.ts:76`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
              await scope.test(name, async (sub: unknown) => {
  ------------------------^
                  started = true;
                  await run(sub as ITestFrameworkContext);
  ...
  
  2026-11-21T14:35:43.450Z error Watch flow=01M7Z8HNQWC6Z9F7B4YG37GK4D/blong realm flow#0 intent=test.blongRealmFlow step getUnknownFlow failed: Missing expe…
  step: getUnknownFlow
  reason: Missing expected rejection: an execution the service never retained is refused rather than drawn empty
  # Subtest: getUnknownFlow
  not ok 1 - Missing expected rejection: an execution the service never retained is refused rather than drawn empty
    ---
    stack: |
      getUnknownFlow (server/test/test/testBlongRealmFlow.ts:76:21)
      executeStepFn (../blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../blong-chain/executor.ts:1174:17)
    at:
      fileName: server/test/test/testBlongRealmFlow.ts
      lineNumber: 76
      columnNumber: 21
      functionName: getUnknownFlow
    type: AssertionError
    generatedMessage: false
  ```

- 🔴 failed **index.test.ts › blong flow (server) › blong realm flow › searchTemplates › the search answers** — `../blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
              await scope.test(name, async (sub: unknown) => {
  ------------------------^
                  started = true;
                  await run(sub as ITestFrameworkContext);
  ...
  
  2026-11-21T14:35:43.426Z error Watch flow=01M7Z8HNQWC6Z9F7B4YG37GK4D/blong realm flow#0 intent=test.blongRealmFlow step searchTemplates failed: the search …
  step: searchTemplates
  reason: the search answers
  # Subtest: searchTemplates
  not ok 1 - the search answers
    ---
    stack: |
      call (../blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../blong-chain/executor.ts:498:44)
      searchTemplates (server/test/test/testBlongRealmFlow.ts:66:28)
      executeStepFn (../blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../blong-chain/executor.ts:1174:17)
    at:
      fileName: ../blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```


## blong-sim-api

- 🔴 failed **index.test.ts › blong sim-api › world time api via sim › timeResult › Cannot read properties of undefined (reading 'datetime')** — `time/server/test/test/testTimeGet.ts:39`

  The raw stream around it:

  ```tap
  root: /home/runner/work/blong/blong/test/blong-sim-api/dist
  2026-11-21T14:35:32.120Z info  Server listening at http://127.0.0.1:8082 [lukaot://t/66dfd34d2658 p=01M7Z8HAV1FXPQECTCPQ3PG4QT]
  2026-11-21T14:35:32.120Z info  Server listening at http://10.1.0.241:8082 [lukaot://t/66dfd34d2658 p=01M7Z8HAWR13SBE5R1E940XZ0K]
  2026-11-21T14:35:32.121Z info  Server listening at http://172.18.0.1:8082 [lukaot://t/66dfd34d2658 p=01M7Z8HAWR13SBE5R1E940XZ0M]
  2026-11-21T14:35:32.255Z error Watch flow=01M7Z8HAXYN6QTEY0VWQVZS7QB/world time api via sim#0 intent=test.time.get step timeResult failed: Cannot read prop…
  step: timeResult
  reason: Cannot read properties of undefined (reading 'datetime')
  # Subtest: blong sim-api
  # Subtest: world time api via sim
  # Subtest: timeResult
  not ok 1 - Cannot read properties of undefined (reading 'datetime')
    ---
    stack: |
      timeResult (time/server/test/test/testTimeGet.ts:39:34)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: time/server/test/test/testTimeGet.ts
      lineNumber: 39
      columnNumber: 34
      functionName: timeResult
    type: TypeError
    tapCaught: returnedPromiseRejection
  ```


## blong-sport

- 🔴 failed **documentFile.play.ts › Sport document file › attaches a PDF, serves it back, and removes it** — `new`
  - trace: `traces/4a73130f-ff64-40eb-8aa1-3fd35b1fae5b-attachment.zip`

## blong-viewer

- 🔴 failed **viewer.play.ts › the page receives wakes over a stream**
  - trace: `traces/5d4b42de-3dac-47ad-8b19-a3940d8c3282-attachment.zip`
