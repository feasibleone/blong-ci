# Failed tests

_feasibleone/blong · workflow Build · build #640_

[Full run](https://github.com/feasibleone/blong/actions/runs/40553852311) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-sport

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
  # Subtest: index.test.ts
      1..0 # no tests found
  not ok 1 - index.test.ts # time=3822.802ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-sport
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-sport/index.test.ts
    exitCode: 1
  ```

