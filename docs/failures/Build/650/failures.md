# Failed tests

_feasibleone/blong · workflow Build · build #650_

[Full run](https://github.com/feasibleone/blong/actions/runs/41132797181) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-gogo

- 🔴 failed **src/gatewayParams.test.ts › src/gatewayParams.test.ts** — `src/gatewayParams.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
          ok 5 - so a rebuilt instance can sign again
          1..5
      ok 5 - a rebuilt gateway over the same source resolves the pair again # time=288.455ms
  
      1..5
      # time=376.97ms
  ok 25 - src/gatewayKeys.test.ts # time=376.97ms
  
  # Subtest: src/gatewayParams.test.ts
      1..0 # no tests found
  not ok 26 - src/gatewayParams.test.ts # time=4034.802ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-gogo
    externalID: src/gatewayParams.test.ts
    command: /opt/hostedtoolcache/node/24.22.1/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-gogo/src/gatewayParams.test.ts
    jobId: 0
  ```

