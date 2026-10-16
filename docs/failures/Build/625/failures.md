# Failed tests

_feasibleone/blong · workflow Build · build #625_

[Full run](https://github.com/feasibleone/blong/actions/runs/38920519444) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-dev

- 🔴 failed **src/memory/memoryFormat.test.ts › src/memory/memoryFormat.test.ts** — `src/memory/memoryFormat.test.ts`

  ```
  test process exited with code unknown
  ```


  The raw stream around it:

  ```tap
          ok 4 - but still writes the item
          1..4
      ok 11 - applyEntries writes the manual list to the root document only # time=8.369ms
  
      1..11
      # time=134.071ms
  ok 23 - src/memory/memoryEdit.test.ts # time=134.071ms
  
  # Subtest: src/memory/memoryFormat.test.ts
      1..0 # no tests found
  not ok 24 - src/memory/memoryFormat.test.ts # time=4089.582ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/tools/blong-dev
    externalID: src/memory/memoryFormat.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/tools/blong-dev/src/memory/memoryFormat.test.ts
    jobId: 2
  ```

