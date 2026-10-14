# Failed tests

_feasibleone/blong · workflow Build · build #618_

[Full run](https://github.com/feasibleone/blong/actions/runs/38617157250) | [Allure report](index.html)

**24 failing test(s) in 7 package(s)**

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
  @@ -1,1 +1,3 @@
  -Array []
  +Array [
  +  "blong-cli: Invalid configuration for blong-cli:",
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

- 🔴 failed **explore.play.ts › access-db — browse tables (SQL via access.table.list)** — `new`
  - trace: `traces/714121e4-4ac3-4da9-b63c-7b31d0360581-attachment.zip`
- 🔴 failed **explore.play.ts › k8s-dev — namespace → category → resource drill-down and item viewer** — `new`
  - trace: `traces/9b66ef5f-6084-44b6-bba0-10369a01d592-attachment.zip`
- 🔴 failed **explore.play.ts › kafka-dev — topics and message viewer** — `new`
  - trace: `traces/3e01143a-2df2-43f7-ad74-90699505b335-attachment.zip`
- 🔴 failed **explore.play.ts › keycloak-dev — realms and users** — `new`
  - trace: `traces/9ce1031c-47da-4be5-83b0-c9a4e529f155-attachment.zip`
- 🔴 failed **explore.play.ts › mongo-dev — databases and collections** — `new`
  - trace: `traces/ed2ae870-3e0a-401a-a967-f6828bbf5313-attachment.zip`
- 🔴 failed **explore.play.ts › navigator mirrors the drill path; ".." and Backspace go up** — `new`
  - trace: `traces/7fcde42c-1920-4d01-a9e4-d43348cd514d-attachment.zip`
- 🔴 failed **explore.play.ts › redis-dev — database index and keys** — `new`
  - trace: `traces/920db17d-261d-4375-8c7a-d3663350b874-attachment.zip`
- 🔴 failed **explore.play.ts › s3-dev — buckets and objects** — `new`
  - trace: `traces/6ff65535-b767-4139-b83a-73e665615e0a-attachment.zip`
- 🔴 failed **explore.play.ts › source list — the commander home** — `new`
  - trace: `traces/557a7b0f-15b0-4947-9720-33730dff6cfe-attachment.zip`
- 🔴 failed **observedBranchList.play.ts › the orchestrator dispatch is drawn with its milestones and its outgoing leg** — `new`
  - trace: `traces/62ec4e74-9cd1-4dff-a20b-ba60375a7852-attachment.zip`
- 🔴 failed **docs.play.ts › Commander documentation images › the source list and one drilled source** — `new`
  - trace: `traces/7a04adb0-4fe3-45af-b911-d82fd5480bf8-attachment.zip`
- 🔴 failed **explore.play.ts › vault-dev — mounts, secrets, and masked secret viewer** — `new`
  - trace: `traces/22f1b69a-1e27-47b9-88e4-81c6f3aa1b31-attachment.zip`

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


## blong-party

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## framework

- 🔴 failed **nscfg/index.test.ts › nscfg/index.test.ts** — `nscfg/index.test.ts`

  ```
  test process exited with code 1
  ```

