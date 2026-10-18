# Failed tests

_feasibleone/blong · workflow Build · build #632_

[Full run](https://github.com/feasibleone/blong/actions/runs/39165952835) | [Allure report](index.html)

**3 failing test(s) in 2 package(s)**

## blong-dev

- 🔴 failed **src/publish/publishGuard.test.ts › no publishing package hides a declared entry point from its tarball › @feasibleone/blong-chain publishes every entry point it declares and has** — `src/publish/publishGuard.test.ts:33`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,3 @@
  -Array []
  +Array [
  +  "browser.ts",
  +]
  ```


  The raw stream around it:

  ```tap
  # time=56.41ms
  ok 31 - src/memory/memoryResolve.test.ts # time=56.41ms
  
  # Subtest: src/publish/publishGuard.test.ts
  # Subtest: no publishing package hides a declared entry point from its tarball
  ok 1 - the repository root is above the working directory
  ok 2 - at least one package declares ci-publish, else this check proves nothing
  ok 3 - @feasibleone/blong could be packed
  ok 4 - @feasibleone/blong publishes every entry point it declares and has
  ok 5 - @feasibleone/blong-chain could be packed
  not ok 6 - @feasibleone/blong-chain publishes every entry point it declares and has
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,3 @@
      -Array []
      +Array [
      +  "browser.ts",
      +]
    at:
      fileName: src/publish/publishGuard.test.ts
      lineNumber: 33
  ```


## blong-lib

- 🔴 failed **layersActivation.test.ts › layersActivation › carries the intents the table declares › a browser test layer is not** — `layersActivation.test.ts:99`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,50 @@
  -/\| `browser\/test` +\| — +\| integration +\|/
  +String(
  +  **Which intent turns a layer on.** Rendered from `WELL_KNOWN_LAYERS` in `core/blong-lib/layers.ts` —
  +  the table the loader itself reads, so this block cannot tell a different story from the runtime.
  +  Read the diagram per intent, and the table per folder.
  +  
  +  ```mermaid
  +  flowchart LR
  +      subgraph SERVER["server platform"]
  +          direction TB
  +          server-default-intent["default"] --- server-default-layers["api · init · meta"]
  +          server-microservice-intent["microservice"] --- server-microservice-layers["error · adapter · orchestrator · gateway · server/api"]
  +          server-k8s-intent["k8s"] --- server-k8s-layers["error · adapter · orchestrator · gateway · server/api"]
  +          server-upgrade-intent["upgrade"] --- server-upgrade-layers["error · adapter · orchestrator"]
  +          server-integration-intent["integration"] --- server-integration-layers["sim · server/test"]
  +      end
  +      subgraph BROWSER["browser platform"]
  +          direction TB
  +          browser-default-intent["default"] --- browser-default-layers["api · init · meta · backend · com
  ```


  The raw stream around it:

  ```tap
  ok 18 - test appears in the table exactly once
  ok 19 - browser/test appears in the table exactly once
  1..19
  ok 1 - renders every well-known layer, once # time=22.888ms
  
  # Subtest: carries the intents the table declares
  ok 1 - the adapter is a runtime layer
  ok 2 - a listener is not a migration one
  ok 3 - microservice groups them
  ok 4 - a browser runtime layer is on by default
  not ok 5 - a browser test layer is not
    ---
    diff: >
      --- expected
  
      +++ actual
  
      @@ -1,1 +1,50 @@
  
      -/\| `browser\/test` +\| — +\| integration +\|/
  
      +String(
  ```

- 🔴 failed **layersActivation.test.ts › layersActivation › the committed page block is what the renderer produces › regenerate with BLONG_UPDATE_DOCS=1 (see the header of this file)** — `layersActivation.test.ts:130`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -17,36 +17,35 @@
       subgraph BROWSER["browser platform"]
           direction TB
           browser-default-intent["default"] --- browser-default-layers["api · init · meta · backend · component · action · actions · browser/api · browser/init · browser/orchestrator"]
           browser-integration-intent["integration"] --- browser-integration-layers["test · browser/test"]
  -        browser-test-ui-intent["test-ui"] --- browser-test-ui-layers["test · browser/test"]
       end
   ```
  
   A layer missing for a platform is simply not auto-discovered there. `default` means the layer loads
   regardless of intents, and every other name is an intent that must be active. `cli` appears in no
   entry here: a command names the layers it needs itself, in the `cli` block of the realm whose
   handlers it     dispatches (D-436).
  
  
  -| Folder                 | Server active in           | Browser active in    |
  -| ---------------------- | -------------------------- | -------------------- |
  -| `api`                  | default                    | default              |
  -| `init`                 | default                    | default              |
  -| `meta`
  ```


  The raw stream around it:

  ```tap
  # Subtest: renders a fixture, so the shape is pinned rather than described
  ok 1 - the diagram is fenced
  ok 2 - the server platform is drawn
  ok 3 - and the browser platform
  ok 4 - a layer active on one platform only
  1..4
  ok 3 - renders a fixture, so the shape is pinned rather than described # time=5.573ms
  
  # Subtest: the committed page block is what the renderer produces
  ok 1 - docs/blong/docs/concepts/layer.md carries the LAYER ACTIVATION marker pair
  not ok 2 - regenerate with BLONG_UPDATE_DOCS=1 (see the header of this file)
    ---
    compare: ===
    at:
      fileName: layersActivation.test.ts
      lineNumber: 130
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (layersActivation.test.ts:130:11)
      Test.<anonymous> (layersActivation.test.ts:119:7)
      layersActivation.test.ts:57:1
    source: |2
  ```

