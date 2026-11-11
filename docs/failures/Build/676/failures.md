# Failed tests

_feasibleone/blong · workflow Build · build #676_

[Full run](https://github.com/feasibleone/blong/actions/runs/43032166272) | [Allure report](index.html)

**43 failing test(s) in 10 package(s)**

## blong-agent

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:42:10.481Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GY9XHEQDCC0X1JP6RK8TR semlog://t/62982d1431ea]
      2026-11-11T14:42:10.482Z info  agent.engine dispatch event adapter.start [semlog://r/01M75GY9XJQW4Z41P2NGBD2RVF semlog://t/8d01ace3e21b]
      2026-11-11T14:42:10.482Z info  agent.notify redis event adapter.start [semlog://r/01M75GY9XJQW4Z41P2NGBD2RVH semlog://t/168e4f34fc58]
      2026-11-11T14:42:10.483Z info  agent.task http event adapter.start [semlog://r/01M75GY9XK7W6Q9PJK464BCM2X semlog://t/02bad641f2e1]
      2026-11-11T14:42:10.484Z info  agent.workspace dispatch event adapter.start [semlog://r/01M75GY9XMCS7T38K0YV88CR71 semlog://t/e57a8c9be847]
      2026-11-11T14:42:10.487Z info  agent.agentDispatch dispatch event adapter.start [semlog://r/01M75GY9XQEWXKEEQFB5CKP4KG semlog://t/14f918735ac3]
      2026-11-11T14:42:10.488Z info  agent.testDispatch dispatch event adapter.start [semlog://r/01M75GY9XRESY787GER42M8PJJ semlog://t/cd14047faa7b]
      2026-11-11T14:42:10.489Z info  testRealm.testDispatch dispatch event adapter.start [semlog://r/01M75GY9XS3AG9GGJQ9NV0CGF7 semlog://t/9581ba1e5768]
      2026-11-11T14:42:10.489Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 1 - index.test.ts # time=3754.384ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-agent
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-agent/index.test.ts
    exitCode: 1
  ```


## blong-chat

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:41:16.245Z info  gateway.meter redis event adapter.start [semlog://r/01M75GWMYNDXVJ311A9RVFK9FG semlog://t/7c73a62befee]
      2026-11-11T14:41:16.246Z info  gateway.testDispatch dispatch event adapter.start [semlog://r/01M75GWMYP0H5QRT1ZB41AZ6N6 semlog://t/7d9560087ba2]
      2026-11-11T14:41:16.248Z info  chat.slack slack event adapter.start [semlog://r/01M75GWMYRB6S1TTAKSAGSJ0GZ semlog://t/8ed63bf187e5]
      2026-11-11T14:41:16.253Z info  chat.viber viber event adapter.start [semlog://r/01M75GWMYWMA4AWT0BVVV1157G semlog://t/c884ac920b1a]
      2026-11-11T14:41:16.258Z info  chat.chatDispatch dispatch event adapter.start [semlog://r/01M75GWMZ2Q17RH3P653JDJ527 semlog://t/876afc1c61f0]
      2026-11-11T14:41:16.259Z info  chat.slackSim webhook event adapter.start [semlog://r/01M75GWMZ3JHNHKC73V559A5EQ semlog://t/5a3d1f49881a]
      2026-11-11T14:41:16.262Z info  chat.viberSim webhook event adapter.start [semlog://r/01M75GWMZ67GCXT7990XE4CPWZ semlog://t/b64732254c02]
      2026-11-11T14:41:16.265Z info  chat.testDispatch dispatch event adapter.start [semlog://r/01M75GWMZ9KM1S8FXVTGSB5HYY semlog://t/bd83cc41dace]
      2026-11-11T14:41:16.265Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 2 - index.test.ts # time=5254.302ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-chat
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-chat/index.test.ts
    jobId: 2
  ```


## blong-feedback

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:39:15.424Z info  srv.subject dispatch event adapter.start [semlog://t/2bc167d5caff]
      2026-11-11T14:39:15.426Z info  login.loginDispatch dispatch event adapter.start [semlog://r/01M75GRYZ2S66Z60N3K8Y0A3ZE semlog://t/e8f99203eb6c]
      2026-11-11T14:39:15.427Z info  core.testDispatch dispatch event adapter.start [semlog://t/b1dcda55f757]
      2026-11-11T14:39:15.428Z info  access.testDispatch dispatch event adapter.start [semlog://r/01M75GRYZ4Q4799QZAZT3NKD93 semlog://t/53ea056b83e4]
      2026-11-11T14:39:15.429Z info  blong.semlog http event adapter.start [semlog://r/01M75GRYZ5XE3JC6SHTX762CD0 semlog://t/d64858a846f2]
      2026-11-11T14:39:15.429Z info  blong.blong dispatch event adapter.start [semlog://r/01M75GRYZ5XE3JC6SHTX762CD2 semlog://t/f9dcbc13356c]
      2026-11-11T14:39:15.430Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GRYZ6E1993XQFYNHMDNNC semlog://t/62982d1431ea]
      2026-11-11T14:39:15.431Z info  feedback.testDispatch dispatch event adapter.start [semlog://r/01M75GRYZ7P3JXD7D9Z00WE2SQ semlog://t/70b15be69f72]
      2026-11-11T14:39:15.431Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 1 - index.test.ts # time=3546.667ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-feedback
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-feedback/index.test.ts
    exitCode: 1
  ```


## blong-int-adapter

- 🔴 failed **(unparsed) › tap exited with code 1 without reporting a failing test**

  ```
  tap exited with code 1 and its own report names no failing test, which is what a run killed by an expired budget or a crash looks like; see tap.raw.tap in the same directory for the reason.
  ```


  The raw stream around it:

  ```tap
  error  vault.generic: Vault Error
  vault.generic: Vault Error
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/vault.ts:329:66)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: listSecrets
  not ok 1 - Vault Error
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/vault.ts:329:66)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```


## blong-kopi

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:36:07.440Z info  login.loginDispatch dispatch event adapter.start [semlog://r/01M75GK7CGA3NNK8SVY3WAK89N semlog://t/e8f99203eb6c]
      2026-11-11T14:36:07.441Z info  core.testDispatch dispatch event adapter.start [semlog://t/b1dcda55f757]
      2026-11-11T14:36:07.442Z info  access.testDispatch dispatch event adapter.start [semlog://r/01M75GK7CJFSSAC4TEN5JJ7ZW0 semlog://t/53ea056b83e4]
      2026-11-11T14:36:07.442Z info  blong.semlog http event adapter.start [semlog://r/01M75GK7CJFSSAC4TEN5JJ7ZW2 semlog://t/d64858a846f2]
      2026-11-11T14:36:07.442Z info  blong.blong dispatch event adapter.start [semlog://r/01M75GK7CJFSSAC4TEN5JJ7ZW4 semlog://t/f9dcbc13356c]
      2026-11-11T14:36:07.443Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GK7CKRDBNYKSQYWNA489Y semlog://t/62982d1431ea]
      2026-11-11T14:36:07.445Z info  $subject.testDispatch dispatch event adapter.start [semlog://r/01M75GK7CNKRCW86E476B1JJKC semlog://t/b75a647af95b]
      2026-11-11T14:36:07.446Z info  testRealm.testDispatch dispatch event adapter.start [semlog://r/01M75GK7CP3MQ4ZSCDR2GV5D0C semlog://t/9581ba1e5768]
      2026-11-11T14:36:07.446Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 1 - index.test.ts # time=4278.825ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-kopi
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
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
      2026-11-11T14:36:10.531Z info  srv.subject dispatch event adapter.start [semlog://t/2bc167d5caff]
      2026-11-11T14:36:10.534Z info  login.loginDispatch dispatch event adapter.start [semlog://r/01M75GKAD6X3HWJ20PQGK7846Y semlog://t/e8f99203eb6c]
      2026-11-11T14:36:10.535Z info  core.testDispatch dispatch event adapter.start [semlog://t/b1dcda55f757]
      2026-11-11T14:36:10.535Z info  access.testDispatch dispatch event adapter.start [semlog://r/01M75GKAD77D1EXT367QRA06ZX semlog://t/53ea056b83e4]
      2026-11-11T14:36:10.536Z info  blong.semlog http event adapter.start [semlog://r/01M75GKAD8YP1W0P08RV92BDBE semlog://t/d64858a846f2]
      2026-11-11T14:36:10.536Z info  blong.blong dispatch event adapter.start [semlog://r/01M75GKAD8YP1W0P08RV92BDBG semlog://t/f9dcbc13356c]
      2026-11-11T14:36:10.537Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GKAD9NS65BVGZHZS5WKVX semlog://t/62982d1431ea]
      2026-11-11T14:36:10.538Z info  kukum.kukum dispatch event adapter.start [semlog://r/01M75GKADA3KTW9QZF0JHYEG17 semlog://t/16331e112750]
      2026-11-11T14:36:10.538Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 3 - index.test.ts # time=3505.246ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-kukum
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-kukum/index.test.ts
    exitCode: 1
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
  ok 1 - the fixtures are regenerated from the templates on every run # time=26.021ms
  
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


## blong-kustomize

- 🔴 failed **index.test.ts › kustomize flow (server) › plan find › planDescribesTheSuite › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › plan find › planIsDeterministic › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › plan find › theOperatorIsAnotherTree › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › aBaseAndItsOverlayMaterializeToTheFlatTree › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › aSplitTreeComposesToTheFlatTree › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › aSplitTreeKeepsTheArtifactOutOfTheBase › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › aWrittenTreeReadsBackAsItself › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › theSerializedTreeIgnoresKeyOrder › Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  error  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  k8s.failed: Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
  at Object.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.exec (/home/runner/work/blong/blong/core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: plan find
  # Subtest: planDescribesTheSuite
  not ok 1 - Kubernetes API error: Error: HTTP protocol is not allowed when skipTLSVerify is not set or false (status none)
    ---
    stack: |
      Object.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.exec (../../core/blong-gogo/src/adapter/server/k8s.ts:1037:48)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
      columnNumber: 35
  ```


## blong-log

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › AllFiltersShowcase › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025390625% different from snapshot (234 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--all-filters-showcase-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › DarkTheme › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025390625% different from snapshot (234 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--dark-theme-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › Empty › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--empty-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ErrorsOnly › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--errors-only-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedExceptionDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-exception-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedHTTPDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-http-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › ExpandedMixedContent › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--expanded-mixed-content-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › FilteredServer › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025390625% different from snapshot (234 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--filtered-server-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPErrorWithBody › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-error-with-body-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPFullDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-full-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPSuccessWithBody › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-success-with-body-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › HTTPWithCacheHeaders › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--http-with-cache-headers-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LargeDataset › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--large-dataset-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LargeDatasetLight › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.027126736111111112% different from snapshot (250 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--large-dataset-light-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › LightTheme › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.026801215277777776% different from snapshot (247 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--light-theme-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingExpanded › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-expanded-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingHTTPAndErrors › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-http-and-errors-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SearchHighlightingSingleLine › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--search-highlighting-single-line-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SingleService › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--single-service-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › SingleTrace › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--single-trace-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › LogViewer › WithHTTPDetails › smoke-test** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
  Error: Expected image to match or be a close match to snapshot but was 0.025716145833333332% different from snapshot (237 differing pixels).
  See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--with-http-details-diff.png
      at postVisit (/home/runner/work/blong/blong/tools/blong-log/.storybook/test-runner.cjs:183:32)
  ```

- 🔴 failed **tools/blong-log/src/client/LogViewer.stories.tsx › tools/blong-log/src/client/LogViewer.stories.tsx — test file failed to run** — `tools/blong-log/src/client/LogViewer.stories.tsx`

  ```
    ● LogViewer › DarkTheme › smoke-test
  
      Expected image to match or be a close match to snapshot but was 0.025390625% different from snapshot (234 differing pixels).
      See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--dark-theme-diff.png
  
        181 |             // Full-page screenshot comparison — saves real PNG files
        182 |             const screenshot = await page.screenshot({fullPage: true});
      > 183 |             expect(screenshot).toMatchImageSnapshot({
            |                                ^
        184 |                 customSnapshotsDir: path.join(
        185 |                     __dirname,
        186 |                     '..',
  
        at postVisit (tools/blong-log/.storybook/test-runner.cjs:183:32)
  
    ● LogViewer › LightTheme › smoke-test
  
      Expected image to match or be a close match to snapshot but was 0.026801215277777776% different from snapshot (247 differing pixels).
      See diff for details: /home/runner/work/blong/blong/tools/blong-log/src/client/__image_snapshots__/__diff_output__/logviewer--light-theme-diff.png
  
        181 |             // Full-page screenshot comparison
  ```


## blong-realm

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:31:58.214Z info  srv.db knex event adapter.start [semlog://r/01M75GBM05Y8RHDX5NVD5V3H65 semlog://t/6032f6ed1930 p=01M75GBKZ8H5X151XYYWMEXW3S]
      2026-11-11T14:31:58.216Z info  srv.subject dispatch event adapter.start [semlog://t/2bc167d5caff]
      2026-11-11T14:31:58.218Z info  login.loginDispatch dispatch event adapter.start [semlog://r/01M75GBM0A0CV5A76GMBKC7WVT semlog://t/e8f99203eb6c]
      2026-11-11T14:31:58.219Z info  core.testDispatch dispatch event adapter.start [semlog://t/b1dcda55f757]
      2026-11-11T14:31:58.220Z info  access.testDispatch dispatch event adapter.start [semlog://r/01M75GBM0CFHMWCCNYWRN5SP36 semlog://t/53ea056b83e4]
      2026-11-11T14:31:58.221Z info  blong.semlog http event adapter.start [semlog://r/01M75GBM0DP4Y01QR2J36ZCZGG semlog://t/d64858a846f2]
      2026-11-11T14:31:58.221Z info  blong.blong dispatch event adapter.start [semlog://r/01M75GBM0DP4Y01QR2J36ZCZGJ semlog://t/f9dcbc13356c]
      2026-11-11T14:31:58.222Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GBM0ESDX62PW1XX7TW369 semlog://t/62982d1431ea]
      2026-11-11T14:31:58.222Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 1 - index.test.ts # time=3466.489ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/core/blong-realm
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/core/blong-realm/index.test.ts
    exitCode: 1
  ```


## blong-sport

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


  The raw stream around it:

  ```tap
      2026-11-11T14:31:45.124Z info  blong.blong dispatch event adapter.start [semlog://r/01M75GB774W82NE0S55P0Y8D8B semlog://t/f9dcbc13356c]
      2026-11-11T14:31:45.125Z info  blong.testDispatch dispatch event adapter.start [semlog://r/01M75GB77528Q2PFMSPE08YR6D semlog://t/62982d1431ea]
      2026-11-11T14:31:45.125Z info  gateway.meter redis event adapter.start [semlog://r/01M75GB77528Q2PFMSPE08YR6F semlog://t/7c73a62befee]
      2026-11-11T14:31:45.127Z info  gateway.testDispatch dispatch event adapter.start [semlog://r/01M75GB777S174QXME17Z2BRWT semlog://t/7d9560087ba2]
      2026-11-11T14:31:45.128Z info  party.testDispatch dispatch event adapter.start [semlog://r/01M75GB778Z5G7PMMQ8XBZSDEV semlog://t/a4b1063314b6]
      2026-11-11T14:31:45.129Z info  sport.testDispatch dispatch event adapter.start [semlog://r/01M75GB779QNYP3JHXFJSNHJRQ semlog://t/a4da1909eaa6]
      2026-11-11T14:31:45.130Z info  feedback.testDispatch dispatch event adapter.start [semlog://r/01M75GB77A1KS3QQ8G426EKAK3 semlog://t/70b15be69f72]
      2026-11-11T14:31:45.132Z info  testRealm.testDispatch dispatch event adapter.start [semlog://r/01M75GB77CEQ8P697TYY2VF6HC semlog://t/9581ba1e5768]
      2026-11-11T14:31:45.132Z info  codec.testDispatch dispatch event adapter.ready [semlog://t/d345e4212ad2]
      1..0 # no tests found
  not ok 1 - index.test.ts # time=4180.456ms
    ---
    stdio: pipe
    cwd: /home/runner/work/blong/blong/realm/blong-sport
    externalID: index.test.ts
    command: /opt/hostedtoolcache/node/24.22.2/x64/bin/node
    args:
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+typescript@3.5.12_@swc+core@1.15.21_@tapjs+core@4.6.0_@swc+core@1.15.…
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+mock@4.4.10_@tapjs+core@4.6.0_@swc+core@1.15.21_@types+node@24.12.0_r…
      - --enable-source-maps
      - --import=file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/@tapjs+processinfo@3.1.12/node_modules/@tapjs/processinfo/dist/esm/import.mjs
      - /home/runner/work/blong/blong/realm/blong-sport/index.test.ts
    exitCode: 1
  ```

