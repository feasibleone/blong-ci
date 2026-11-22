# Failed tests

_feasibleone/blong · workflow Build · build #712_

[Full run](https://github.com/feasibleone/blong/actions/runs/45072412869) | [Allure report](index.html)

**3 failing test(s) in 3 package(s)**

## blong-dev

- 🔴 failed **src/repo/runtimeImportGuard.test.ts › no realm, suite or demo source imports the runtime › the runtime is a binary, not a dependency — reach a helper through the package a realm may import (`@feasibleone/blong/…`), and keep the reasoning in memory** — `src/repo/runtimeImportGuard.test.ts:98`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,3 @@
  -Array []
  +Array [
  +  "demo/blong-generate/generate.tool.ts:20",
  +]
  ```


  The raw stream around it:

  ```tap
  1..1
  ok 2 - the guard reports a package’s source ignored by the root file, not by its own # time=14.237ms
  
  1..2
  # time=89.465ms
  ok 46 - src/repo/ignoredSourceGuard.test.ts # time=89.465ms
  
  # Subtest: src/repo/runtimeImportGuard.test.ts
  # Subtest: no realm, suite or demo source imports the runtime
  ok 1 - the repository root is above the working directory
  not ok 2 - the runtime is a binary, not a dependency — reach a helper through the package a realm may import (`@feasibleone/blong/…`), and keep the rea…
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,3 @@
      -Array []
      +Array [
      +  "demo/blong-generate/generate.tool.ts:20",
      +]
    at:
      fileName: src/repo/runtimeImportGuard.test.ts
      lineNumber: 98
  ```


## blong-lib

- 🔴 failed **layersActivation.test.ts › layersActivation › the committed page block is what the renderer produces › regenerate with BLONG_UPDATE_DOCS=1 (see the header of this file)** — `layersActivation.test.ts:130`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -11,9 +11,8 @@
           server-default-intent["default"] --- server-default-layers["api · init · meta"]
           server-microservice-intent["microservice"] --- server-microservice-layers["error · lukaot · adapter · orchestrator · gateway · server/api"]
           server-k8s-intent["k8s"] --- server-k8s-layers["error · lukaot · adapter · orchestrator · gateway · server/api"]
           server-upgrade-intent["upgrade"] --- server-upgrade-layers["error · lukaot · adapter · orchestrator"]
  -        server-dev-intent["dev"] --- server-dev-layers["server/api"]
           server-integration-intent["integration"] --- server-integration-layers["sim · server/test"]
       end
       subgraph BROWSER["browser platform"]
           direction TB
  @@ -44,9 +43,9 @@
   | `lukaot`               | microservice, k8s, upgrade | —                    |
   | `adapter`              | microservice, k8s, upgrade | —                    |
   | `orchestrator`         | microservice, k8s, upgrade | —                    |
   | `gateway`              | microservice, k8s          | —                    |
  -| `server/api`           | microservice, k8s, dev     | —                    |
  +|
  ```


  The raw stream around it:

  ```tap
  # Subtest: renders a fixture, so the shape is pinned rather than described
  ok 1 - the diagram is fenced
  ok 2 - the server platform is drawn
  ok 3 - and the browser platform
  ok 4 - a layer active on one platform only
  1..4
  ok 3 - renders a fixture, so the shape is pinned rather than described # time=1.9ms
  
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


## blong-sport

- 🟡 flaky **reference.play.ts › Reference › create sport sport** — `new`
  - trace: `traces/6526df25-d305-40f3-9634-83a2f0022f2a-attachment.zip`
