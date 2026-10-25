# Failed tests

_feasibleone/blong · workflow Build · build #635_

[Full run](https://github.com/feasibleone/blong/actions/runs/40211522445) | [Allure report](index.html)

**5 failing test(s) in 3 package(s)**

## blong-commander

- 🔴 failed **explore.play.ts › vault-dev — mounts, secrets, and masked secret viewer** — `new`
  - trace: `traces/1d86b895-b277-4fb2-9d88-839bc9cbd686-attachment.zip`

## blong-dev

- 🔴 failed **src/docs/storybookSites.test.ts › the register in the repository matches what the command reads › sport exists** — `src/docs/storybookSites.test.ts:84`

  The raw stream around it:

  ```tap
      t.test('the register in the repository matches what the command reads', t => {
          const sites = loadStorybookSites(repoRoot(import.meta.dirname));
          t.same(
      ------^
              sites.map(site => site.name),
              ['browser', 'suite', 'log'],
    ...
  
  ok 2 - browser exists
  ok 3 - suite exists
  not ok 4 - sport exists
    ---
    at:
      fileName: src/docs/storybookSites.test.ts
      lineNumber: 84
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (src/docs/storybookSites.test.ts:84:11)
      src/docs/storybookSites.test.ts:76:3
    source: >2
          );
          for (const site of sites) {
  ```

- 🔴 failed **src/docs/storybookSites.test.ts › the register in the repository matches what the command reads › the checkout publishes three Storybooks** — `src/docs/storybookSites.test.ts:78`

  ```
  --- expected
  +++ actual
  @@ -1,5 +1,6 @@
   Array [
     "browser",
     "suite",
  +  "sport",
     "log",
   ]
  ```


  The raw stream around it:

  ```tap
  ok 4 - and changes nothing
  1..4
  ok 17 - sortSection drops exact duplicates and is idempotent # time=3.902ms
  
  1..17
  # time=153.443ms
  ok 12 - src/cspell/cspellConfig.test.ts # time=153.443ms
  
  # Subtest: src/docs/storybookSites.test.ts
  # Subtest: the register in the repository matches what the command reads
  not ok 1 - the checkout publishes three Storybooks
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,5 +1,6 @@
       Array [
         "browser",
         "suite",
      +  "sport",
         "log",
       ]
    at:
  ```


## blong-sport

- 🔴 failed **olympic.play.ts › Olympic › browse sport campaign**
  - trace: `traces/7da8672d-44a1-468d-92be-6fa77a722ddf-attachment.zip`
- 🔴 failed **competition.play.ts › Competition › browse sport competition**
  - trace: `traces/43d1ce1a-af5c-4437-baeb-0a0f0a1ab9c0-attachment.zip`
