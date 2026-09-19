# Failed tests

_feasibleone/blong · workflow Build · build #568_

[Full run](https://github.com/feasibleone/blong/actions/runs/35467128002) | [Allure report](index.html)

**27 failing test(s) in 9 package(s)**

## blong-cli

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › and nothing was logged to stderr** — `index.test.ts:35`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,41 @@
  -
  +2026-09-19T20:37:18.662Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP6FP50HJN76WWH7EQ6CM8 t=semantic-log://template/801b9e485f3f]
  +2026-09-19T20:37:18.749Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP6FRXAMXNJFQNJ3MSFT1P t=semantic-log://template/d123e9aa4055]
  +2026-09-19T20:37:18.788Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP6FT4T40H3EY6KJH1NSW6 t=semantic-log://template/97218ffb936e p=01M2XP6FRXAMXNJFQNJ3MSFT1P]
  +2026-09-19T20:37:18.789Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP6FT5M2BKJ4KTHZYD4R2J t=semantic-log://temp
  ```

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › exits clean** — `index.test.ts:33`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › the result is the only thing on stdout** — `index.test.ts:34`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -hello-world
  +
  ```

- 🔴 failed **index.test.ts › a handler error is reported without a stack trace on stdout › the message is on stderr** — `index.test.ts:78`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,44 @@
  -/provide --value=TEXT or --file=PATH/
  +String(
  +  2026-09-19T20:37:58.135Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7P7KNCJWA84GWCTW4VKQ t=semantic-log://template/801b9e485f3f]
  +  2026-09-19T20:37:58.251Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7PBB1KA7CNGPTJ4EHD8Z t=semantic-log://template/d123e9aa4055]
  +  2026-09-19T20:37:58.304Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7PD08CE4FYY2KFTWD1V5 t=semantic-log://template/97218ffb936e p=01M2XP7PBB1KA7CNGPTJ4EHD8Z]
  +  2026-09-19T20:37:58.305Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7PD19RYCS51
  ```

- 🔴 failed **index.test.ts › the exit code says whether the command did what was asked › and says which method it could not find** — `index.test.ts:64`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,44 @@
  -/unknown method 'text\.bogus\.get'/
  +String(
  +  2026-09-19T20:37:47.830Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7C5NF1BV7PPBAWRKQ6AW t=semantic-log://template/801b9e485f3f]
  +  2026-09-19T20:37:47.918Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7C8EV0T0643CS32YJGXK t=semantic-log://template/d123e9aa4055]
  +  2026-09-19T20:37:47.961Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7C9R3QBBMK0PZ0ZWYDY0 t=semantic-log://template/97218ffb936e p=01M2XP7C8EV0T0643CS32YJGXK]
  +  2026-09-19T20:37:47.961Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XP7C9S10HFHEDJN
  ```

- 🔴 failed **index.test.ts › the machine channel stays parseable › exits clean** — `index.test.ts:42`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › the machine channel stays parseable › Unexpected end of JSON input** — `index.test.ts:43`
- 🔴 failed **index.test.ts › the platform is available, so a command can read a file › exits clean** — `index.test.ts:53`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **index.test.ts › the platform is available, so a command can read a file › the file is read through `this.platform` and rendered for a terminal** — `index.test.ts:54`

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


## blong-gateway

- 🔴 failed **observedFlow.play.ts › a flow this realm served is drawn as a diagram**
  - trace: `traces/a3d8a2e9-e16a-4296-b6a4-10d4c82a6628-attachment.zip`

## blong-gogo

- 🔴 failed **src/exit.intent.test.ts › timeout!** — `src/exit.intent.test.ts`

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
  - trace: `traces/ee6bf35a-f671-4c3e-8b67-c927dbf8a98a-attachment.zip`
- 🔴 failed **blong.play.ts › open blong.template.browse**
  - trace: `traces/81344451-12f0-412d-bd87-9c681a74c04a-attachment.zip`

## blong-suite

- 🔴 failed **portalMerge.play.ts › the suite portal carries both realms’ menus**
  - trace: `traces/4f6ce2cb-00d9-4395-b188-b21116faa658-attachment.zip`

## framework

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **nscfg/index.test.ts › nscfg/index.test.ts** — `nscfg/index.test.ts`

  ```
  test process exited with code 1
  ```


## semantic-log

- 🔴 failed **test/flow/faults.test.ts › F2: a retry burst is one template at a rate-shift, not 41 new templates (PRD R6b, R12) › and it is stamped on the template the payer repeated rather than on a new one** — `test/flow/faults.test.ts:365`
