# Failed tests

_feasibleone/blong · workflow Build · build #571_

[Full run](https://github.com/feasibleone/blong/actions/runs/35598694674) | [Allure report](index.html)

**34 failing test(s) in 4 package(s)**

## blong-int-adapter

- 🔴 failed **k8s.test.ts › blong int-adapter › k8s namespace list › listNamespaces › Kubernetes Error** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **k8s.test.ts › blong int-adapter › k8s pod log explore › findPods › Kubernetes Error** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **k8s.test.ts › blong int-adapter › k8s pod log explore › readPodLog › Kubernetes Error** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **keycloak.test.ts › blong int-adapter › keycloak realm CRUD › addRealm › Keycloak authentication failed** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **keycloak.test.ts › blong int-adapter › keycloak realm CRUD › editRealm › timeout!** — `keycloak.test.ts`
- 🔴 failed **keycloak.test.ts › blong int-adapter › keycloak realm CRUD › findRealms › Keycloak authentication failed** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **keycloak.test.ts › blong int-adapter › keycloak realm CRUD › getRealm › timeout!** — `keycloak.test.ts`
- 🔴 failed **keycloak.test.ts › blong int-adapter › keycloak realm list › listRealms › Keycloak authentication failed** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis explore list › listKeys › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis hash vocabulary › delField › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis hash vocabulary › getAllFields › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis hash vocabulary › getField › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis hash vocabulary › incrByField › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis hash vocabulary › setFields › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › delKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › existsKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › expireKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › getKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › getMissing › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › setKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis key vocabulary › ttlKey › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis script vocabulary › evalNoKeys › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **redis.test.ts › blong int-adapter › redis script vocabulary › evalScript › Redis unavailable** — `../../core/blong-gogo/src/error.ts:191`
- 🔴 failed **mysql.test.ts › mysql.test.ts** — `mysql.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **kafka.test.ts › timeout!** — `kafka.test.ts`
- 🔴 failed **mongodb.test.ts › timeout!** — `mongodb.test.ts`

## blong-kopi

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```


## blong-kukum

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added browser group ran** — `e2e.test.ts:186`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/e2e flow browser › addGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: add** — `e2e.test.ts:184`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/(^| › )addGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the added server test ran: find** — `e2e.test.ts:185`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -/(^| › )findGadget$/m
  +"# e2e-realm: 0 passed, 1 failed (1 total)"
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the realm suite exits 0** — `e2e.test.ts:172`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```

- 🔴 failed **e2e.test.ts › the realm runs its server and browser tests over the added entity › the report records no failing test** — `e2e.test.ts:182`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -0
  +1
  ```


## blong-realm

- 🔴 failed **index.test.ts › index.test.ts** — `index.test.ts`

  ```
  test process exited with code 1
  ```

