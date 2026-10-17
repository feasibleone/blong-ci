# Failed tests

_feasibleone/blong · workflow Build · build #627_

[Full run](https://github.com/feasibleone/blong/actions/runs/39035957574) | [Allure report](index.html)

**2 failing test(s) in 1 package(s)**

## blong-dev

- 🔴 failed **src/report/allurePublish.test.ts › publishAllureReport merges every producer into one report › and the bundle is published with it** — `src/report/allurePublish.test.ts:114`

  The raw stream around it:

  ```tap
    source: >2
          const page = readFileSync(publishedPage, 'utf8');
          t.equal(page.includes('data:text/javascript'), false, 'the bundle is not inlined');
          t.match(page, /src="\.\/allure-main-[0-9a-f]{16}\.js"/, 'the page points at a file beside it');
      ------^
          t.ok(published.mainBundle, 'the result names the bundle the page loads');
          t.ok(
    ...
  
  ok 13 - the result names the bundle the page loads
  not ok 14 - and the bundle is published with it
    ---
    at:
      fileName: src/report/allurePublish.test.ts
      lineNumber: 114
      columnNumber: 7
      typeName: Test
    stack: |
      Test.<anonymous> (src/report/allurePublish.test.ts:114:7)
    source: >2
          t.match(page, /src="\.\/allure-main-[0-9a-f]{16}\.js"/, 'the page points at a file beside it');
          t.ok(published.mainBundle, 'the result names the bundle the page loads');
          t.ok(
  ```

- 🔴 failed **src/report/allurePublish.test.ts › publishAllureReport merges every producer into one report › the page points at a file beside it** — `src/report/allurePublish.test.ts:112`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/src="\.\/allure-main-[0-9a-f]{16}\.js"/
  +"<!doctype html><html><body><script   src=\"../../../_assets/allure/allure-main-26e545fd9d7c90ff.js\"></script></body></html>"
  ```


  The raw stream around it:

  ```tap
  ok 2 - both producers went into it
  ok 3 - should be equal
  ok 4 - both producers results are in the one directory Allure renders
  ok 5 - the trace archive moved to the published directory
  ok 6 - and out of what the single-file report embeds
  ok 7 - should be equal
  ok 8 - the published report is a single file
  ok 9 - should be equal
  ok 10 - the report was published
  ok 11 - the bundle is not inlined
  not ok 12 - the page points at a file beside it
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -/src="\.\/allure-main-[0-9a-f]{16}\.js"/
      +"<!doctype html><html><body><script   src=\"../../../_assets/allure/allure-main-26e545fd9d7c90ff.js\"></script></body></html>"
    at:
      fileName: src/report/allurePublish.test.ts
      lineNumber: 112
      columnNumber: 7
      typeName: Test
  ```

