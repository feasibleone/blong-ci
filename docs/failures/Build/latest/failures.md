# Failed tests

_feasibleone/blong · workflow Build · build #599_

[Full run](https://github.com/feasibleone/blong/actions/runs/38061058646) | [Allure report](index.html)

**10 failing test(s) in 3 package(s)**

## blong-ci-report

- 🔴 failed **index.test.ts › renderCiReport leaves the deltas out when there is no baseline › counts, time and coverage stand on their own** — `index.test.ts:664`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,18 @@
  -/^\| fake-fail \| ❌ \| 8 \| 2 \| 0 \| — \| 10 \| 1m 05s ⏱️ logs in as the seeded user 11s \| 25% \|$/m
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests**
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — |
  +  | fake-fail | ❌ | 8 | 2 | 0 | — | 10 | 20s ⏱️ logs in as the seeded user 11s | 25% |
  +  | fake-flaky | ⚠️ | 2 | 0 | 1 | 1 | 4 | 8.2s ⏱️ handles a cold cache 5.1s | — |
  +  | fake-pass | ✅ | 12 | 0 | 0 | — | 12 | 1.9s | 80% |
  +  | fake-silent | — | — | — | — | — | — | — | 50% |
  +  
  +)
  ```

- 🔴 failed **index.test.ts › renderCiReport leaves the deltas out when there is no baseline › the run cost is stated without a delta** — `index.test.ts:662`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,18 @@
  -/· 2m 15s of test time\*\*/
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests**
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — |
  +  | fake-fail | ❌ | 8 | 2 | 0 | — | 10 | 20s ⏱️ logs in as the seeded user 11s | 25% |
  +  | fake-flaky | ⚠️ | 2 | 0 | 1 | 1 | 4 | 8.2s ⏱️ handles a cold cache 5.1s | — |
  +  | fake-pass | ✅ | 12 | 0 | 0 | — | 12 | 1.9s | 80% |
  +  | fake-silent | — | — | — | — | — | — | — | 50% |
  +  
  +)
  ```

- 🔴 failed **index.test.ts › renderCiReport merges metrics, coverage, deltas and links into one table › a grown package: test delta, faster than before, coverage up** — `index.test.ts:536`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,35 @@
  -/^\| fake-pass \| ✅ \| 12 \| 0 \| 0 \| — \| 12 \(\+2\) \| 4\.2s \(-3\.8s\) \| 🟢 80% \(\+10\.0pp\) \| — \|$/m
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests** — build #551
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  *vs last merged main: tests 32 (+12), coverage 44.3% (+11.0pp)*
  +  
  +  📊 [Coverage report](https://example.test/blong-ci/coverage/Build/551/) · 🤖 Failure report: [this run](https://example.test/blong-ci/failures/Build/551/failures.json) · [latest](https://example.test/blong-ci/failures/Build/latest/failures.json)
  +  
  +  > 1 package(s) produced no test report.
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  > Failures: 2 new (green on main) · 1 already failing there · 1 intermittent there.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage | Report |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — | — |
  +  | fake-fail | ❌
  ```

- 🔴 failed **index.test.ts › renderCiReport merges metrics, coverage, deltas and links into one table › a regressed package links its published report** — `index.test.ts:546`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,35 @@
  -/^\| fake-fail \| ❌ \| 8 \| 2 \| 0 \| — \| 10 \(\+2\) \| 1m 05s \(\+5\.0s\) ⏱️ logs in as the seeded user 11s \| 🔴 25% \(-5\.0pp\) \| \[report\]\(https:\/\/example\.test\/blong-ci\/fake-fail\/Build\/551\/\) \|$/m
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests** — build #551
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  *vs last merged main: tests 32 (+12), coverage 44.3% (+11.0pp)*
  +  
  +  📊 [Coverage report](https://example.test/blong-ci/coverage/Build/551/) · 🤖 Failure report: [this run](https://example.test/blong-ci/failures/Build/551/failures.json) · [latest](https://example.test/blong-ci/failures/Build/latest/failures.json)
  +  
  +  > 1 package(s) produced no test report.
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  > Failures: 2 new (green on main) · 1 already failing there · 1 intermittent there.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage | Report |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- |
  +  | fake-both (tap 4 302ms · pl
  ```

- 🔴 failed **index.test.ts › renderCiReport merges metrics, coverage, deltas and links into one table › a two-runner package names its legs, and its slowest test sits in the duration cell** — `index.test.ts:541`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,35 @@
  -/^\| fake-both \(tap 4 · playwright 2 ❌\) \| ❌ \| 4 \| 1 \| 0 \| 1 \| 6 \| 54s ⏱️ opens the roles tab 8\.2s \| — \| — \|$/m
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests** — build #551
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  *vs last merged main: tests 32 (+12), coverage 44.3% (+11.0pp)*
  +  
  +  📊 [Coverage report](https://example.test/blong-ci/coverage/Build/551/) · 🤖 Failure report: [this run](https://example.test/blong-ci/failures/Build/551/failures.json) · [latest](https://example.test/blong-ci/failures/Build/latest/failures.json)
  +  
  +  > 1 package(s) produced no test report.
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  > Failures: 2 new (green on main) · 1 already failing there · 1 intermittent there.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage | Report |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — | — |
  +  |
  ```

- 🔴 failed **index.test.ts › renderCiReport merges metrics, coverage, deltas and links into one table › an unmoved coverage number carries no mark** — `index.test.ts:577`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,31 @@
  -/^\| fake-pass \| ✅ \| 12 \| 0 \| 0 \| — \| 12 \(\+2\) \| 4\.2s \(-3\.8s\) \| 80% \(0\.0pp\) \|/m
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests**
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  *vs last merged main: tests 32 (+12), coverage 44.3% (+11.0pp)*
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  > Failures: 2 new (green on main) · 1 already failing there · 1 intermittent there.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — |
  +  | fake-fail | ❌ | 8 | 2 | 0 | — | 10 (+2) | 20s ⏱️ logs in as the seeded user 11s | 🔴 25% (-5.0pp) |
  +  | fake-flaky | ⚠️ | 2 | 0 | 1 | 1 | 4 | 8.2s ⏱️ handles a cold cache 5.1s | — |
  +  | fake-pass | ✅ | 12 | 0 | 0 | — | 12 (+2) | 1.9s | 80% (0.0pp) |
  +  | fake-silent | — | — | — | — | — | — | — | 🟡 50% (-0.4pp) |
  +  
  +  ### Failed suites (4 test(s))
  +
  ```

- 🔴 failed **index.test.ts › renderCiReport merges metrics, coverage, deltas and links into one table › totals line carries the counts, what the run cost, and how that compares** — `index.test.ts:505`

  ```
  --- expected
  +++ actual
  @@ -1,1 +1,35 @@
  -/\*\*4 package\(s\) · 26 passed, 3 failed, 1 flaky \(32 total\) · 2m 15s \(\+15s\) of test time\*\* — build #551/
  +String(
  +  ## CI Summary
  +  
  +  **4 package(s) · 26 passed, 3 failed, 1 flaky (32 total) · 47s of test time, 1m 28s outside the tests** — build #551
  +  
  +  *by runner: tap 20 · playwright 12 (3 failed)*
  +  
  +  *vs last merged main: tests 32 (+12), coverage 44.3% (+11.0pp)*
  +  
  +  📊 [Coverage report](https://example.test/blong-ci/coverage/Build/551/) · 🤖 Failure report: [this run](https://example.test/blong-ci/failures/Build/551/failures.json) · [latest](https://example.test/blong-ci/failures/Build/latest/failures.json)
  +  
  +  > 1 package(s) produced no test report.
  +  
  +  > 1 skipped, 1 todo in 2 package(s): fake-both 1, fake-flaky 1.
  +  
  +  > Failures: 2 new (green on main) · 1 already failing there · 1 intermittent there.
  +  
  +  | Package | Result | Passed | Failed | Flaky | Not run | Total | Duration | Coverage | Report |
  +  | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- |
  +  | fake-both (tap 4 302ms · playwright 2 16s ❌) | ❌ | 4 | 1 | 0 | 1 | 6 | 17s ⏱️ opens the roles tab 8.2s | — | — |
  +  | fake-fail
  ```


## blong-commander

- 🔴 failed **explore.play.ts › keycloak-dev — realms and users** — `new`
  - trace: `traces/088c6963-8925-40fd-a760-dc086064441b-attachment.zip`

## blong-party

- 🔴 failed **index.test.ts › blong-party registration flow (browser) › acl diagnostics › A table with nothing wrong reports nothing › matrixReportsNothing_s2 › timeout!** — `index.test.ts`
- 🔴 failed **index.test.ts › blong-party registration flow (browser) › timeout!** — `index.test.ts`
