# Failed tests

_feasibleone/blong · workflow Build · build #626_

[Full run](https://github.com/feasibleone/blong/actions/runs/38935179269) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-ttk

- 🔴 failed **integration.test.ts › integration.test.ts** — `integration.test.ts`

  ```
  test process exited with signal SIGILL
  ```


  The raw stream around it:

  ```tap
          ok 3 - nested partyIdInfo present
          1..3
      ok 47 - emitCollection - deeply nested body triggers multi-line object # time=12.054ms
  
      1..47
      # time=2898.652ms
  ok 1 - index.test.ts # time=2898.652ms
  
  # Subtest: integration.test.ts
      1..0 # no tests found
  not ok 2 - integration.test.ts # time=15754.163ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/tools/blong-ttk
    externalID: integration.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/tools/blong-ttk/integration.test.ts
    jobId: 2
  ```

