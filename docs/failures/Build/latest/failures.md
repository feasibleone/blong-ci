# Failed tests

_feasibleone/blong · workflow Build · build #596_

[Full run](https://github.com/feasibleone/blong/actions/runs/37990995033) | [Allure report](index.html)

**14 failing test(s) in 4 package(s)**

## blong-commander

- 🔴 failed **explore.play.ts › k8s-dev — namespace → category → resource drill-down and item viewer** — `new`
  - trace: `traces/928af5e9-d1a1-4fa0-8615-350d8ec35645-attachment.zip`
- 🟡 flaky **explore.play.ts › keycloak-dev — realms and users** — `new`
  - trace: `traces/d2834eac-02b4-453a-8dbc-f1a32368cb5d-attachment.zip`

## blong-dev

- 🔴 failed **src/memory/hindsight/hindsightPage.test.ts › a documentation page carries the taxonomy the entries are told apart by › it is a documentation page** — `src/memory/hindsight/hindsightPage.test.ts:75`
- 🔴 failed **src/memory/hindsight/hindsightPage.test.ts › a skill carries the procedural tags › it is an agent skill** — `src/memory/hindsight/hindsightPage.test.ts:103`
- 🔴 failed **src/memory/hindsight/hindsightSources.test.ts › sourceTags names the tags a reconcile owns › the pages** — `src/memory/hindsight/hindsightSources.test.ts:58`

  ```
  --- expected
  +++ actual
  @@ -1,4 +1,4 @@
   Array [
  -  "type:documentation",
  -  "type:agent-skill",
  +  "kind:documentation",
  +  "kind:agent-skill",
   ]
  ```

- 🔴 failed **src/commands/memory.test.ts › the memory command layer › a page ingest sends the pages under their own ids and tags › a page carries the documentation tag** — `src/commands/memory.test.ts:384`
- 🔴 failed **src/commands/memory.test.ts › the memory command layer › a search across sources asks with a tag group › the sources are alternatives — a flat list would be an AND and match nothing** — `src/commands/memory.test.ts:329`

  ```
  --- expected
  +++ actual
  @@ -1,16 +1,16 @@
   Array [
     Object {
       "or": Array [
         Object {
           "tags": Array [
             "memory",
           ],
         },
         Object {
           "tags": Array [
  -          "type:documentation",
  +          "kind:documentation",
           ],
         },
       ],
     },
   ]
  ```

- 🔴 failed **src/commands/memory.test.ts › the memory command layer › a search for pages asks with the page tag, not the entry tag › a page search never carries the entry tag, so it cannot drift back to entries** — `src/commands/memory.test.ts:313`

  ```
  --- expected
  +++ actual
  @@ -1,3 +1,3 @@
   Array [
  -  "type:documentation",
  +  "kind:documentation",
   ]
  ```


## blong-gateway

- 🔴 failed **index.test.ts › blong-gateway meter flow (browser) › gateway meter http flow › rateProbeBlocked › rate probe third call was blocked** — `browser/test/test/testMeterHttpFlow.ts:220`

  ```
  simple
  ```


## blong-party

- 🔴 failed **index.test.ts › blong-party registration flow (browser) › acl diagnostics › A wrong matrix cell is marked where the reader looks › matrixMismatchIsInItsCell_s0 › timeout!** — `index.test.ts`
- 🔴 failed **index.test.ts › blong-party registration flow (browser) › acl matrix application › The party.person.get application matrix › assert the party.person.get matrix_s0 › timeout!** — `index.test.ts`
- 🔴 failed **index.test.ts › blong-party registration flow (browser) › cannot create subtest after parent test ends** — `../../core/blong-chain/index.ts:622`
- 🔴 failed **index.test.ts › blong-party registration flow (browser) › cannot create subtest after parent test ends** — `../../core/blong-chain/index.ts:622`
- 🔴 failed **index.test.ts › blong-party registration flow (browser) › cannot create subtest after parent test ends** — `../../core/blong-chain/index.ts:622`
