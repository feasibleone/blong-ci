# Failed tests

_feasibleone/blong · workflow Build · build #667_

[Full run](https://github.com/feasibleone/blong/actions/runs/42258885506) | [Allure report](index.html)

**17 failing test(s) in 7 package(s)**

## blong-access

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › addRole › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › addUser › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › cleanup › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › editRoleBit › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › editUser › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › findUsers › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › getRole › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```

- 🔴 failed **index.test.ts › blong-access login flow (server) › access model flow › getUserDetails › Role bit 8 is already used by the role Access Customer** — `../../core/blong-gogo/src/error.ts:191`

  The raw stream around it:

  ```tap
  role.bitTaken: Role bit 8 is already used by the role Access Customer
  at Proxy.handler (/home/runner/work/blong/blong/core/blong-gogo/src/error.ts:191:35)
  at AdapterBase.accessRoleEnsure (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleEnsure.ts:65:30)
  at process.processTicksAndRejections (node:internal/process/task_queues:104:5)
  at async AdapterBase.accessRoleAdd (/home/runner/work/blong/blong/realm/blong-access/adapter/db/accessRoleAdd.ts:34:37)
  at async answered (/home/runner/work/blong/blong/core/blong-gogo/src/AdapterBase.ts:422:32)
  at async exec (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:270:24)
  at async <anonymous> (/home/runner/work/blong/blong/core/blong-gogo/src/loop.ts:18:27)
  at async file:///home/runner/work/blong/blong/common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
  # Subtest: addRole
  not ok 1 - Role bit 8 is already used by the role Access Customer
    ---
    stack: |
      Proxy.handler (../../core/blong-gogo/src/error.ts:191:35)
      AdapterBase.accessRoleEnsure (adapter/db/accessRoleEnsure.ts:65:30)
      AdapterBase.accessRoleAdd (adapter/db/accessRoleAdd.ts:34:37)
      answered (../../core/blong-gogo/src/AdapterBase.ts:422:32)
      exec (../../core/blong-gogo/src/loop.ts:270:24)
      <anonymous> (../../core/blong-gogo/src/loop.ts:18:27)
      ../../common/temp/node_modules/.pnpm/p-queue@9.1.0/node_modules/p-queue/dist/index.js:394:36
    at:
      fileName: ../../core/blong-gogo/src/error.ts
      lineNumber: 191
  ```


## blong-commander

- 🔴 failed **observedBranchList.play.ts › the orchestrator dispatch is drawn with its milestones and its outgoing leg** — `new`
  - trace: `traces/0c76d687-5758-4e52-8540-acd1df159bb3-attachment.zip`

## blong-gateway

- 🔴 failed **observedFlow.play.ts › a flow this realm served is drawn as a diagram** — `new`
  - trace: `traces/1d47ed62-464e-4245-ba60-e4d83c596047-attachment.zip`

## blong-kopi

- 🔴 failed **$subject.play.ts › $Object › browse $subject $object** — `new`
  - trace: `traces/37d980a5-c4ad-45fd-acd2-804e995d0a48-attachment.zip`
- 🔴 failed **$subject.play.ts › $Object › cleanup $subject $object** — `new`
  - trace: `traces/9865ebe6-0380-47fd-ad15-a13b914b13c5-attachment.zip`
- 🔴 failed **$subject.play.ts › $Object › create $subject $object** — `new`
  - trace: `traces/eb4b4076-86c6-4f3a-a52b-968af41df774-attachment.zip`
- 🔴 failed **$subject.play.ts › $Object › edit $subject $object** — `new`
  - trace: `traces/a9532973-d5cd-4127-9085-4be80930ad24-attachment.zip`

## blong-party

- 🔴 failed **selfRegistration.play.ts › self-registration: create account and auto-login** — `new`
  - trace: `traces/b6e4da40-74ac-4161-ad62-207c5e9ff8a0-attachment.zip`

## blong-realm

- 🔴 failed **blong.play.ts › a role without the capability › is refused, not shown an empty page** — `new`
  - trace: `traces/1018a3dc-447f-48dd-aaf5-ab7d840143a2-attachment.zip`

## blong-sport

- 🟡 flaky **bgModels.play.ts › bg create cycle +5 (empty form)** — `new`
  - trace: `traces/36168bf8-ab07-4d9a-834c-5fade73a6777-attachment.zip`
