# Failed tests

_feasibleone/blong · workflow Build · build #629_

[Full run](https://github.com/feasibleone/blong/actions/runs/39057849500) | [Allure report](index.html)

**23 failing test(s) in 8 package(s)**

## blong-access

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        elapsedMs: 6751
        progress: {"done":1,"total":1}
      2026-10-17T18:39:14.556Z warn  blong-access browser operation "start testClient" took 6753ms [semlog://t/3c1d1ab0c5c9]
        label: start testClient
        elapsedMs: 6753
        progress: {"done":1,"total":1}
      2026-10-17T18:39:14.600Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:39:14.647Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      2026-10-17T18:39:14.698Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/browser/orchestrator/subject [semlog://t/5479766abf…
      1..0 # no tests found
  not ok 2 - index.test.ts # time=14275.681ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-access
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-access/index.test.ts
    jobId: 0
  ```


## blong-commander

- 🔴 failed **commander.test.ts › commander.test.ts** — `commander.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:37:38.195Z warn  commander server operation "start adapter" took 6706ms [semlog://t/aea41419e0e3]
        label: start adapter
        elapsedMs: 6706
        progress: {"done":1,"total":1}
      2026-10-17T18:37:38.236Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:37:38.272Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      1..0 # no tests found
  not ok 2 - commander.test.ts # time=14349.368ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-commander
    externalID: commander.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-commander/commander.test.ts
    jobId: 0
  ```


## blong-gateway

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        elapsedMs: 7402
        progress: {"done":1,"total":1}
      2026-10-17T18:36:29.695Z warn  blong-gateway browser operation "start testClient" took 7467ms [semlog://t/31d54b7e4a38]
        label: start testClient
        elapsedMs: 7467
        progress: {"done":1,"total":1}
      2026-10-17T18:36:29.775Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:36:29.897Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      2026-10-17T18:36:30.032Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/browser/orchestrator/subject [semlog://t/5479766abf…
      1..0 # no tests found
  not ok 1 - index.test.ts # time=15451.884ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-gateway
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-gateway/index.test.ts
    exitCode: 1
  ```


## blong-int-adapter

- 🔴 failed **http.test.ts › http.test.ts** — `http.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **k8s.test.ts › k8s.test.ts** — `k8s.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **kafka.test.ts › kafka.test.ts** — `kafka.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **keycloak.test.ts › keycloak.test.ts** — `keycloak.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **mongodb.test.ts › mongodb.test.ts** — `mongodb.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **mysql.test.ts › mysql.test.ts** — `mysql.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **redis.test.ts › redis.test.ts** — `redis.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **s3.test.ts › s3.test.ts** — `s3.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```

- 🔴 failed **vault.test.ts › vault.test.ts** — `vault.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:35:56.379Z info  int-adapter config event config.load [semlog://t/b73fff5acded]
        files: []
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:36:08.527Z warn  int-adapter server operation "start adapter" took 10701ms [semlog://t/d1ec4523433c]
        label: start adapter
        elapsedMs: 10701
        progress: {"done":1,"total":1}
      2026-10-17T18:36:08.543Z error Watch Error loading /home/runner/work/blong/blong/test/blong-int-adapter/vault/test/fixtures/secret.ts ; probably a generic …
      1..0 # no tests found
  not ok 9 - vault.test.ts # time=21745.115ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/test/blong-int-adapter
    externalID: vault.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/test/blong-int-adapter/vault.test.ts
    jobId: 2
  ```


## blong-kopi

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        label: start testClient
        elapsedMs: 4570
        progress: {"done":1,"total":1}
      2026-10-17T18:34:51.595Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/browser/orchestrator/subject [semlog://t/5479766abf…
      2026-10-17T18:34:51.636Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-kopi/orchestrator/subject [semlog://t/1a0137c63429]
      2026-10-17T18:34:51.707Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:34:51.740Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-access/browser/orchestrator/component [semlog://t/b83efdf…
      2026-10-17T18:34:51.745Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      2026-10-17T18:34:51.854Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-access/browser/orchestrator/subject [semlog://t/18a92757d…
      1..0 # no tests found
  not ok 1 - index.test.ts # time=9829.625ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-kopi
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-kopi/index.test.ts
    exitCode: 1
  ```


## blong-kukum

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        env: ["BLONG_MASTER_KEY"]
        argv: []
      2026-10-17T18:35:01.727Z warn  blong-kukum server operation "start adapter" took 4753ms [semlog://t/17ec46d0db2f]
        label: start adapter
        elapsedMs: 4753
        progress: {"done":1,"total":1}
      2026-10-17T18:35:01.750Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-kukum/orchestrator/kukum [semlog://t/30551628684f]
      2026-10-17T18:35:01.868Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:35:01.905Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      1..0 # no tests found
  not ok 3 - index.test.ts # time=9729.21ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-kukum
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-kukum/index.test.ts
    exitCode: 1
  ```

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the added entity was browsed** — `e2e.test.ts:281`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,33 @@
  -/Gadget › browse/
  +String(
  +  [WebServer] 2026-10-17T18:34:46.153Z info  e2e-realm config event config.load [semlog://t/a2aa1bb62a56]
  +  [WebServer]   files: []
  +  [WebServer]   env: ["BLONG_MASTER_KEY"]
  +  [WebServer]   argv: ["gateway","resolution"]
  +  [WebServer] 2026-10-17T18:34:49.171Z warn  e2e-realm server operation "start adapter" took 2741ms [semlog://t/2c582a460636]
  +  [WebServer]   label: start adapter
  +  [WebServer]   elapsedMs: 2741
  +  [WebServer]   progress: {"done":1,"total":1}
  +  [WebServer] 2026-10-17T18:34:49.187Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-kukum/test/fixture/e2e-realm/orchestrator/subject [semlog://t/5322dd3044d5]
  +  [WebServer] 2026-10-17T18:34:49.200Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
  +  [WebServer] 2026-10-17T18:34:49.214Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
  +  Error: Process from config.webServer was not able to start. Exit code: 1
  +  
  +  Allure report: .ci-report/publish (1 producer(s), ../../../
  ```


  The raw stream around it:

  ```tap
              t.match(output, new RegExp(`${ADDED_NAME} › browse`), 'the added entity was browsed');
          },
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -0
      +1
    ...
  
  not ok 3 - the added entity was browsed
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,33 @@
      -/Gadget › browse/
      +String(
      +  [WebServer] 2026-10-17T18:34:46.153Z info  e2e-realm config event config.load [semlog://t/a2aa1bb62a56]
      +  [WebServer]   files: []
      +  [WebServer]   env: ["BLONG_MASTER_KEY"]
      +  [WebServer]   argv: ["gateway","resolution"]
      +  [WebServer] 2026-10-17T18:34:49.171Z warn  e2e-realm server operation "start adapter" took 2741ms [semlog://t/2c582a460636]
  ```

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the Playwright suite exits 0** — `e2e.test.ts:280`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


  The raw stream around it:

  ```tap
      {skip: skipped},
  ...
  
  # Subtest: every added primitive is covered by those tests
  ok 1 - all 10 artifacts are covered
  1..1
  ok 3 - every added primitive is covered by those tests # time=1.178ms
  
  # Subtest: the Playwright leg drives the model page against committed baselines
  ok 1 - the added entity has committed baselines
  not ok 2 - the Playwright suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 280
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:280:11)
    source: >2
              }
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added browser group ran** — `e2e.test.ts:196`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/e2e flow browser › addGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```


  The raw stream around it:

  ```tap
      Test.<anonymous> (e2e.test.ts:195:11)
    source: >2
              const names = [summary, ...passed].join('\n');
              t.match(names, /(^| › )addGadget$/m, 'the added server test ran: add');
              t.match(names, /(^| › )findGadget$/m, 'the added server test ran: find');
      ----------^
              t.match(names, /e2e flow browser › addGadget$/m, 'the added browser group ran');
          },
    ...
  
  not ok 7 - the added browser group ran
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -/e2e flow browser › addGadget$/m
      +"# e2e-realm: 0 passed, 1 failed (1 total)"
    at:
      fileName: e2e.test.ts
      lineNumber: 196
      columnNumber: 11
      typeName: Test
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: add** — `e2e.test.ts:194`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/(^| › )addGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```


  The raw stream around it:

  ```tap
              const names = [summary, ...passed].join('\n');
              t.match(names, /(^| › )addGadget$/m, 'the added server test ran: add');
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -0
      +1
    ...
  
  not ok 5 - the added server test ran: add
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -/(^| › )addGadget$/m
      +"# e2e-realm: 0 passed, 1 failed (1 total)"
    at:
      fileName: e2e.test.ts
      lineNumber: 194
      columnNumber: 11
      typeName: Test
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: find** — `e2e.test.ts:195`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/(^| › )findGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```


  The raw stream around it:

  ```tap
      Test.<anonymous> (e2e.test.ts:194:11)
    source: >2
              t.equal(failed, 0, 'the report records no failing test');
              const names = [summary, ...passed].join('\n');
              t.match(names, /(^| › )addGadget$/m, 'the added server test ran: add');
      ----------^
              t.match(names, /(^| › )findGadget$/m, 'the added server test ran: find');
              t.match(names, /e2e flow browser › addGadget$/m, 'the added browser group ran');
    ...
  
  not ok 6 - the added server test ran: find
    ---
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -/(^| › )findGadget$/m
      +"# e2e-realm: 0 passed, 1 failed (1 total)"
    at:
      fileName: e2e.test.ts
      lineNumber: 195
      columnNumber: 11
      typeName: Test
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the realm suite exits 0** — `e2e.test.ts:179`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


  The raw stream around it:

  ```tap
  ok 2 - regenerated meta/type/gadget.ts
  ok 3 - regenerated server/test/test/testGadget.ts
  ok 4 - regenerated browser/test/test/testGadget.flow.ts
  ok 5 - regenerated meta/model/e2eGadgetModel.ts
  ok 6 - every generated test group was registered
  ok 7 - the committed baselines survived the regeneration
  1..7
  ok 1 - the fixtures are regenerated from the templates on every run # time=41.297ms
  
  # Subtest: the realm runs its server and browser tests over the added entity
  not ok 1 - the realm suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 179
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:179:11)
    source: >2
              }
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the report records no failing test** — `e2e.test.ts:192`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


  The raw stream around it:

  ```tap
    diff: |
      --- expected
      +++ actual
      @@ -1,1 +1,1 @@
      -0
      +1
    ...
  
  ok 2 - no tap failures in the console output
  ok 3 - the tap leg reported into the package (the report holds every runner that did)
  not ok 4 - the report records no failing test
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 192
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:192:11)
    source: >2
                  'the tap leg reported into the package (the report holds every runner that did)',
              );
  ```


## blong-party

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
        elapsedMs: 6038
        progress: {"done":0,"total":1}
      2026-10-17T18:32:30.923Z warn  blong-party browser operation "start testClient" took 6049ms [semlog://t/0eea0861c281]
        label: start testClient
        elapsedMs: 6049
        progress: {"done":1,"total":1}
      2026-10-17T18:32:30.943Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:32:30.994Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      2026-10-17T18:32:31.065Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/browser/orchestrator/subject [semlog://t/5479766abf…
      1..0 # no tests found
  not ok 1 - index.test.ts # time=11403.289ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-party
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-party/index.test.ts
    exitCode: 1
  ```


## blong-realm

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-10-17T18:32:16.666Z warn  blong-realm browser operation "start testClient" took 5401ms [semlog://t/d77ff394e014]
        label: start testClient
        elapsedMs: 5401
        progress: {"done":1,"total":1}
      2026-10-17T18:32:16.758Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/browser/orchestrator/subject [semlog://t/5479766abf…
      2026-10-17T18:32:16.794Z info  ApiSchema Generating dir /home/runner/work/blong/blong/core/blong-server/orchestrator/subject [semlog://t/66909e9b3825]
      2026-10-17T18:32:16.825Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-login/orchestrator/login [semlog://t/e2340bcc4d9e]
      2026-10-17T18:32:17.046Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-access/browser/orchestrator/component [semlog://t/b83efdf…
      2026-10-17T18:32:17.062Z info  ApiSchema Generating dir /home/runner/work/blong/blong/realm/blong-access/browser/orchestrator/subject [semlog://t/18a92757d…
      1..0 # no tests found
  not ok 1 - index.test.ts # time=11137.764ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-realm
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.21.0/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-realm/index.test.ts
    exitCode: 1
  ```

