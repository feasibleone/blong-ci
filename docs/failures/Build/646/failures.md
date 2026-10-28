# Failed tests

_feasibleone/blong · workflow Build · build #646_

[Full run](https://github.com/feasibleone/blong/actions/runs/40704663961) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-gogo

- 🔴 failed **src/adapter/schema/knex/json.test.ts › src/adapter/schema/knex/json.test.ts** — `src/adapter/schema/knex/json.test.ts`

  ```
  test process exited with signal SIGILL
  ```


  The raw stream around it:

  ```tap
          ok 1 - backtick doubled in identifier
          1..1
      ok 5 - ensureDatabase — escapes backticks in the database name # time=0.927ms
  
      1..5
      # time=174.969ms
  ok 2 - src/adapter/schema/knex/database.test.ts # time=174.969ms
  
  # Subtest: src/adapter/schema/knex/json.test.ts
      1..0 # no tests found
  not ok 3 - src/adapter/schema/knex/json.test.ts # time=10988.772ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-gogo
    externalID: src/adapter/schema/knex/json.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-gogo/src/adapter/schema/knex/json.test.ts
    jobId: 0
  ```

