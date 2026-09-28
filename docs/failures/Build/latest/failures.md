# Failed tests

_feasibleone/blong · workflow Build · build #587_

[Full run](https://github.com/feasibleone/blong/actions/runs/36445568265) | [Allure report](index.html)

**59 failing test(s) in 19 package(s)**

## blong-access

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-cli

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › and nothing of its own reached stderr** — `index.test.ts:62`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,16 @@
  -Array []
  +Array [
  +  "node:internal/modules/run_main:107",
  +  "    triggerUncaughtException(",
  +  "    ^",
  +  "Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/home/runner/work/blong/blong/demo/blong-cli/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/demo/blong-cli/cli.ts",
  +  "    at finalizeResolution (node:internal/modules/esm/resolve:272:11)",
  +  "    at moduleResolve (node:internal/modules/esm/resolve:879:10)",
  +  "    at defaultResolve (node:internal/modules/esm/resolve:1006:11)",
  +  "    at nextResolve (node:internal/modules/esm/hooks:785:28)",
  +  "    at AsyncLoaderHooksOnLoaderHookWorker.resolve (node:internal/modules/esm/hooks:269:30)",
  +  "    at MessagePort.handleMessage (node:internal/modules/esm/worker:251:24)",
  +  "    at [nodejs.internal.kHybridDispatch] (node:internal/event_target:848:20)",
  +  "    at MessagePort.<anonymous> (node:internal/per_context/messageport:23:28) {",
  +  "}",
  +  "Node.js v24.21.0",
  +]
  ```

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › exits clean** — `index.test.ts:60`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › the result is the only thing on stdout** — `index.test.ts:61`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -hello-world
  +
  ```

- 🔴 failed **index.test.ts › a handler error is reported without a stack trace on stdout › the message is on stderr** — `index.test.ts:105`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,21 @@
  -/provide --value=TEXT or --file=PATH/
  +String(
  +  
  +  node:internal/modules/run_main:107
  +      triggerUncaughtException(
  +      ^
  +  Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/home/runner/work/blong/blong/demo/blong-cli/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/demo/blong-cli/cli.ts
  +      at finalizeResolution (node:internal/modules/esm/resolve:272:11)
  +      at moduleResolve (node:internal/modules/esm/resolve:879:10)
  +      at defaultResolve (node:internal/modules/esm/resolve:1006:11)
  +      at nextResolve (node:internal/modules/esm/hooks:785:28)
  +      at AsyncLoaderHooksOnLoaderHookWorker.resolve (node:internal/modules/esm/hooks:269:30)
  +      at MessagePort.handleMessage (node:internal/modules/esm/worker:251:24)
  +      at [nodejs.internal.kHybridDispatch] (node:internal/event_target:848:20)
  +      at MessagePort.<anonymous> (node:internal/per_context/messageport:23:28) {
  +    code: 'ERR_MODULE_NOT_FOUND',
  +    url: 'file:///home/runner/work/blong/blong/demo/blong-cli/node_modules/@feasibleone/blong/dist/types.js'
  +  }
  +  
  +  Node.js v24.21.0
  +  
  +)
  ```

- 🔴 failed **index.test.ts › the exit code says whether the command did what was asked › --help is not a failure** — `index.test.ts:97`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › the exit code says whether the command did what was asked › and says which method it could not find** — `index.test.ts:91`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,21 @@
  -/unknown method 'text\.bogus\.get'/
  +String(
  +  
  +  node:internal/modules/run_main:107
  +      triggerUncaughtException(
  +      ^
  +  Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/home/runner/work/blong/blong/demo/blong-cli/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/demo/blong-cli/cli.ts
  +      at finalizeResolution (node:internal/modules/esm/resolve:272:11)
  +      at moduleResolve (node:internal/modules/esm/resolve:879:10)
  +      at defaultResolve (node:internal/modules/esm/resolve:1006:11)
  +      at nextResolve (node:internal/modules/esm/hooks:785:28)
  +      at AsyncLoaderHooksOnLoaderHookWorker.resolve (node:internal/modules/esm/hooks:269:30)
  +      at MessagePort.handleMessage (node:internal/modules/esm/worker:251:24)
  +      at [nodejs.internal.kHybridDispatch] (node:internal/event_target:848:20)
  +      at MessagePort.<anonymous> (node:internal/per_context/messageport:23:28) {
  +    code: 'ERR_MODULE_NOT_FOUND',
  +    url: 'file:///home/runner/work/blong/blong/demo/blong-cli/node_modules/@feasibleone/blong/dist/types.js'
  +  }
  +  
  +  Node.js v24.21.0
  +  
  +)
  ```

- 🔴 failed **index.test.ts › the machine channel stays parseable › exits clean** — `index.test.ts:69`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › the machine channel stays parseable › Unexpected end of JSON input** — `index.test.ts:70`
- 🔴 failed **index.test.ts › the platform is available, so a command can read a file › exits clean** — `index.test.ts:80`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › the platform is available, so a command can read a file › the file is read through `this.platform` and rendered for a terminal** — `index.test.ts:81`

  ```
  --- expected
  +++ actual
  @@ -1,5 +1,3 @@
   Array [
  -  "lines: 2",
  -  "words: 5",
  -  "characters: 24",
  +  "",
   ]
  ```


## blong-commander

- 🔴 failed **commander.test.ts › commander.test.ts** — `commander.test.ts`

  ```
  test process exited with code 1
  ```


## blong-cucumber

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-eip

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-gateway

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-gogo

- 🔴 failed **src/graceful-shutdown.spawn.test.ts › blong CLI exits 0 with the shutdown marker after timeout sends SIGTERM › exit code 0 (graceful shutdown), got 1** — `src/graceful-shutdown.spawn.test.ts:64`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **src/graceful-shutdown.spawn.test.ts › blong CLI exits 0 with the shutdown marker after timeout sends SIGTERM › stderr contains the shutdown marker** — `src/graceful-shutdown.spawn.test.ts:65`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,23 @@
  -/blong: shutting down on SIGTERM/
  +String(
  +  node:internal/modules/esm/resolve:272
  +      throw new ERR_MODULE_NOT_FOUND(
  +            ^
  +  
  +  Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/home/runner/work/blong/blong/core/blong-gogo/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/core/blong-gogo/src/adapter/schema/knex/binary.ts
  +      at finalizeResolution (node:internal/modules/esm/resolve:272:11)
  +      at moduleResolve (node:internal/modules/esm/resolve:879:10)
  +      at defaultResolve (node:internal/modules/esm/resolve:1006:11)
  +      at #cachedDefaultResolve (node:internal/modules/esm/loader:705:20)
  +      at #resolveAndMaybeBlockOnLoaderThread (node:internal/modules/esm/loader:725:38)
  +      at ModuleLoader.resolveSync (node:internal/modules/esm/loader:763:56)
  +      at #resolve (node:internal/modules/esm/loader:687:17)
  +      at ModuleLoader.getOrCreateModuleJob (node:internal/modules/esm/loader:607:35)
  +      at ModuleJob.syncLink (node:internal/modules/esm/module_job:276:33)
  +      at ModuleJob.link (node:internal/modules/esm/module_job:381:17) {
  +    code: 'ERR_MODULE_NOT_FOUND',
  ```

- 🔴 failed **src/graceful-shutdown.spawn.test.ts › blong CLI exits 0 with the shutdown marker after timeout sends SIGTERM › teardown ran (adapter.stop events fired)** — `src/graceful-shutdown.spawn.test.ts:66`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,7 @@
  -/adapter\.stop/
  +String(
  +  2026-09-28T15:50:11.966Z warn  blong-hello server operation "start adapter" took 1001ms [semlog://t/f7566fdfa431]
  +    label: start adapter
  +    elapsedMs: 1001
  +    progress: {"done":0,"total":1}
  +  
  +)
  ```

- 🔴 failed **src/ci.intent.test.ts › src/ci.intent.test.ts** — `src/ci.intent.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **src/exit.intent.test.ts › src/exit.intent.test.ts** — `src/exit.intent.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **src/frameworkRealms.test.ts › src/frameworkRealms.test.ts** — `src/frameworkRealms.test.ts`

  ```
  test process exited with code 1
  ```


## blong-int-adapter

- 🔴 failed **http.test.ts › http.test.ts** — `http.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **k8s.test.ts › k8s.test.ts** — `k8s.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **kafka.test.ts › kafka.test.ts** — `kafka.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **keycloak.test.ts › keycloak.test.ts** — `keycloak.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **mongodb.test.ts › mongodb.test.ts** — `mongodb.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **mysql.test.ts › mysql.test.ts** — `mysql.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **redis.test.ts › redis.test.ts** — `redis.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **s3.test.ts › s3.test.ts** — `s3.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **vault.test.ts › vault.test.ts** — `vault.test.ts`

  ```
  test process exited with code 1
  ```


## blong-int-sql

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-kopi

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-kukum

- 🔴 failed **e2e.test.ts › e2e.test.ts** — `e2e.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **libraries.test.ts › libraries.test.ts** — `libraries.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **operations.test.ts › operations.test.ts** — `operations.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **scaffold.test.ts › scaffold.test.ts** — `scaffold.test.ts`

  ```
  test process exited with code 1
  ```


## blong-party

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-realm

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-sim-api

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-sim-tcp

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-ttk

- 🔴 failed **index.test.ts › callback register → wait → receive full coordination flow › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackRegister.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callback register throws on duplicate correlationId › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackRegister.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callback store coordination › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackRegister.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackCallbackWait rejects on timeout › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackRegister.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackCallbackWait throws when no prior register › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackWait.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackReceive returns not-found for unregistered correlationId › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackReceive.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackRuleDispatch - matches rule and returns decision › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackRuleDispatch.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackRuleDispatch - method mismatch does not match rule › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackRuleDispatch.ts** — `index.test.ts`
- 🔴 failed **index.test.ts › callbackRuleDispatch - returns mockCallback when no rules match › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackRuleDispatch.ts** — `index.test.ts`
- 🔴 failed **integration.test.ts › integration - callback coordination › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/callback/orchestrator/callback/callbackCallbackRegister.ts** — `integration.test.ts`
- 🔴 failed **integration.test.ts › integration - execute example collection with TestExecutor › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/examples/collections/simple-transfer.ts** — `integration.test.ts`
- 🔴 failed **migration.test.ts › migration - migrateMigrateHelperExtract finds shared operations › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/migrate/orchestrator/migrate/migrateMigrateHelperExtract.ts** — `migration.test.ts`
- 🔴 failed **migration.test.ts › migration e2e - migrateMigrateCollectionConvert full pipeline with syntax check › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/migrate/orchestrator/migrate/migrateMigrateCollectionConvert.ts** — `migration.test.ts`
- 🔴 failed **index.test.ts › server.ts exports default › Cannot find module '/home/runner/work/blong/blong/tools/blong-ttk/node_modules/@feasibleone/blong/dist/types.js' imported from /home/runner/work/blong/blong/tools/blong-ttk/server.ts** — `index.test.ts`

## config-hot-reload

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## framework

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **nscfg/index.test.ts › nscfg/index.test.ts** — `nscfg/index.test.ts`

  ```
  test process exited with code 1
  ```


## handler-test-poc

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

