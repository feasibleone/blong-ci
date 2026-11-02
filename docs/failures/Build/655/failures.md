# Failed tests

_feasibleone/blong · workflow Build · build #655_

[Full run](https://github.com/feasibleone/blong/actions/runs/41413779453) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-gogo

- 🔴 failed **src/adapter/server/folderShape.test.ts › every handler group under adapter/server is a folder of handlers › slack/markdown.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered** — `src/adapter/server/folderShape.test.ts:94`

  The raw stream around it:

  ```tap
  ok 2 - engine/ is served by engine.ts — a group folder named after something else hides which base its handlers belong to
  ok 3 - slack/ is served by slack.ts — a group folder named after something else hides which base its handlers belong to
  ok 4 - viber/ is served by viber.ts — a group folder named after something else hides which base its handlers belong to
  ok 5 - workspace/ is served by workspace.ts — a group folder named after something else hides which base its handlers belong to
  ok 6 - engine/engineAccountCheck.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registe…
  ok 7 - engine/engineSessionClose.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registe…
  ok 8 - engine/engineSessionRun.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered
  ok 9 - engine/engineStepRun.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered
  ok 10 - slack/acknowledge.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered
  ok 11 - slack/blocks.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered
  not ok 12 - slack/markdown.ts has a default export — a plain module in a group folder is reported as a mis-filing and its method is never registered
    ---
    at:
      fileName: src/adapter/server/folderShape.test.ts
      lineNumber: 94
      columnNumber: 15
      typeName: Test
    stack: |
      Test.<anonymous> (src/adapter/server/folderShape.test.ts:94:15)
    source: >2
              for (const name of files) {
                  const loaded = await load(folder, name);
                  t.ok(
  ```

