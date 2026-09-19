# Failed tests

_feasibleone/blong · workflow Build · build #567_

[Full run](https://github.com/feasibleone/blong/actions/runs/35464494945) | [Allure report](index.html)

**28 failing test(s) in 9 package(s)**

## blong-cli

- 🔴 failed **index.test.ts › a command dispatches in-process and prints its result on stdout › and nothing was logged to stderr** — `index.test.ts:35`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,41 @@
  -
  +2026-09-19T20:00:25.734Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM2YM59V1PPBZQ4D5HJE11 t=semantic-log://template/801b9e485f3f]
  +2026-09-19T20:00:25.781Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM2YNNDQH99F8QQBHJQGWS t=semantic-log://template/d123e9aa4055]
  +2026-09-19T20:00:25.803Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM2YPBTK3314P15HFRGW6M t=semantic-log://template/97218ffb936e p=01M2XM2YNNDQH99F8QQBHJQGWS]
  +2026-09-19T20:00:25.803Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM2YPBTK3314P15HFRGW6N t=semantic-log://temp
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
  +  2026-09-19T20:00:49.185Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3NH0HEMZ1B10Y68BT5G7 t=semantic-log://template/801b9e485f3f]
  +  2026-09-19T20:00:49.256Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3NK8Z2BQCMEFAE0K8K7R t=semantic-log://template/d123e9aa4055]
  +  2026-09-19T20:00:49.337Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3NNSPKXK89T83V9BNKZK t=semantic-log://template/97218ffb936e p=01M2XM3NK8Z2BQCMEFAE0K8K7R]
  +  2026-09-19T20:00:49.338Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3NNTD4RR6FW
  ```

- 🔴 failed **index.test.ts › the exit code says whether the command did what was asked › and says which method it could not find** — `index.test.ts:64`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,44 @@
  -/unknown method 'text\.bogus\.get'/
  +String(
  +  2026-09-19T20:00:42.959Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-core/adapter/db/core.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3FEE9FQGNBB9EVXZ8CYZ t=semantic-log://template/801b9e485f3f]
  +  2026-09-19T20:00:43.004Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/accessModel.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3FFWFVW345WS6DK7ANES t=semantic-log://template/d123e9aa4055]
  +  2026-09-19T20:00:43.027Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/account.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3FGKGEQAPJ0YMNC340ZG t=semantic-log://template/97218ffb936e p=01M2XM3FFWFVW345WS6DK7ANES]
  +  2026-09-19T20:00:43.028Z error Watch Error loading /home/runner/work/blong/blong/realm/blong-access/adapter/db/oidc.ts ; probably a generic source code was put in a handler group folder [r=semantic-log://record/01M2XM3FGMNJZF0GE0D
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
  - trace: `traces/2a901196-f988-4383-9744-e1f05f70ba30-attachment.zip`

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

- 🔴 failed **blong.play.ts › an observed execution is drawn as a diagram**
  - trace: `traces/a4886dda-6cf8-4083-822c-a016bc85fd2d-attachment.zip`
- 🔴 failed **blong.play.ts › open blong.digest.browse**
  - trace: `traces/df616cee-f6a4-4c2f-8537-e7d4e16b5ffb-attachment.zip`
- 🔴 failed **blong.play.ts › open blong.template.browse**
  - trace: `traces/22b862e3-6741-4af9-8aad-749f3aa1310b-attachment.zip`

## blong-suite

- 🔴 failed **portalMerge.play.ts › the suite portal carries both realms’ menus**
  - trace: `traces/8baad60b-4918-4168-86b8-be446e26deb4-attachment.zip`

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


## semantic-log

- 🔴 failed **test/flow/faults.test.ts › F2: a retry burst is one template at a rate-shift, not 41 new templates (PRD R6b, R12) › and it is stamped on the template the payer repeated rather than on a new one** — `test/flow/faults.test.ts:365`
