# Failed tests

_feasibleone/blong · workflow Build · build #569_

[Full run](https://github.com/feasibleone/blong/actions/runs/35495226743) | [Allure report](index.html)

**6 failing test(s) in 5 package(s)**

## blong-gateway

- 🔴 failed **observedFlow.play.ts › a flow this realm served is drawn as a diagram**
  - trace: `traces/a628362c-20cd-49a4-b523-3ca1c45f48c0-attachment.zip`

## blong-kukum

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the Playwright suite exits 0** — `e2e.test.ts:270`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


## blong-realm

- 🔴 failed **blong.play.ts › open blong.digest.browse**
  - trace: `traces/a51f38c6-22e8-4623-aa8d-4d79350b0e54-attachment.zip`
- 🔴 failed **blong.play.ts › open blong.template.browse**
  - trace: `traces/f3ea1537-c11b-4b2e-be19-c26f96a69b3e-attachment.zip`

## blong-suite

- 🔴 failed **portalMerge.play.ts › the suite portal carries both realms’ menus**
  - trace: `traces/48d1f263-81ba-4f40-9546-b67b02a17cd9-attachment.zip`

## blong-party

- 🟡 flaky **organization.play.ts › Party Organization › browse party organization**
  - trace: `traces/a35986a9-4d53-4bfb-ad44-417ff47b1c69-attachment.zip`
