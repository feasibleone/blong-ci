# Failed tests

_feasibleone/blong · workflow Build · build #576_

[Full run](https://github.com/feasibleone/blong/actions/runs/35740713322) | [Allure report](index.html)

**6 failing test(s) in 4 package(s)**

## blong-commander

- 🔴 failed **explore.play.ts › vault-dev — mounts, secrets, and masked secret viewer**
  - trace: `traces/6f1ad6cc-7cf4-4cf6-ba60-ebbf8d4a5a0c-attachment.zip`

## blong-gogo

- 🔴 failed **src/adapter/schema/knex/database.test.ts › src/adapter/schema/knex/database.test.ts** — `src/adapter/schema/knex/database.test.ts`

  ```
  test process exited with code unknown
  ```


## blong-realm

- 🔴 failed **blong.play.ts › open blong.digest.browse**
  - trace: `traces/06f73829-8f8b-426a-9cfd-abf92678bc35-attachment.zip`

## semantic-log

- 🔴 failed **test/flow/observedFlows.test.ts › the docs page carries each block a run produced (D14) › inter: the page carries the block a run produced, in the page's own formatting** — `test/flow/observedFlows.test.ts:368`
- 🔴 failed **test/flow/observedFlows.test.ts › the docs page carries each block a run produced (D14) › single: the page carries the block a run produced, in the page's own formatting** — `test/flow/observedFlows.test.ts:368`
- 🔴 failed **test/flow/observedFlows.test.ts › the published flow shapes are what a run observes (PRD R23) › the artifact is what a run produced, not what a document said it should be — regenerate with SEMANTIC_LOG_UPDATE_DIAGRAMS=1** — `test/flow/observedFlows.test.ts:327`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -64,12 +64,12 @@
   | call | caller → receiver | phase | position | declared | answered | declared in |
   | ---- | ----------------- | ----- | -------- | -------- | -------- | ----------- |
   | `discovery.parties` | `payer` → `hub` | discovery | 1 | 1 | 1 | `flow/payer.ts:67` |
   | `discovery.payee` | `hub` → `payee` | discovery | 1.1 | 1 | 1 | `flow/hub.ts:56` |
  -| `quote.rates` | `payer` → `hub` | quote | 2 | 1 | 1 | `flow/payer.ts:85` |
  +| `quote.rates` | `payer` → `hub` | quote | 2 | 1 | 1 | `flow/payer.ts:84` |
   | `quote.fx` | `hub` → `fxp` | quote | 2.1 | 1 | 1 | `flow/hub.ts:57` |
   | `quote.payee` | `hub` → `payee` | quote | 2.2 | 1 | 1 | `flow/hub.ts:58` |
  -| `transfer.submit` | `payer` → `hub` | transfer | 3 | 1 | 1 | `flow/payer.ts:124` |
  +| `transfer.submit` | `payer` → `hub` | transfer | 3 | 1 | 1 | `flow/payer.ts:123` |
   | `transfer.deliver` | `hub` → `payee` | transfer | 3.1 | 1 | 1 | `flow/hub.ts:59` |
   <!-- END OBSERVED FLOWS: transfer.single -->
   <!-- BEGIN OBSERVED FLOWS: transfer.inter -->
   Participants: `payer`, `hubA`, `proxy`, `hubB`, `payee`, `fxp`. 13 calls observed across 1 execution(s).
  @@ -119,14 +119,14 @@
   |
  ```

