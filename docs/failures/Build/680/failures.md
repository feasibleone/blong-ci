# Failed tests

_feasibleone/blong · workflow Build · build #680_

[Full run](https://github.com/feasibleone/blong/actions/runs/43319630347) | [Allure report](index.html)

**6 failing test(s) in 6 package(s)**

## blong-int-adapter

- 🔴 failed **mysql.test.ts › blong int-adapter › mysql CRUD › findWithOptions › findWithOptions** — `../../core/blong-chain/executor.ts:995`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,14 +1,14 @@
   String(
     Array [
       Object {
  -      "unitDescription": "First blong integration test widget",
  +      "unitDescription": "Created via upsert in integration test",
         "unitId": "<masked>",
  -      "unitName": "Widget Alpha",
  +      "unitName": "Widget Merged",
       },
       Object {
  -      "unitDescription": "Second blong integration test widget",
  +      "unitDescription": "First blong integration test widget",
         "unitId": "<masked>",
  -      "unitName": "Widget Beta",
  +      "unitName": "Widget Alpha",
       },
     ]
   )
  ```


  The raw stream around it:

  ```tap
  # Subtest: insertUnits
  1..0
  ok 12 - insertUnits # time=8.587ms
  
  # Subtest: verifyInsert
  1..0
  ok 13 - verifyInsert # time=9.948ms
  
  2026-11-12T22:46:13.103Z warn  mysql.sql knex flow=01M78Z1AFH2JBNY5XD8QJ80KY5/-#-1 leg=sql.unit.find#1 [sql.unit.find] ignoring order by "unitName": no suc…
  # Subtest: findWithOptions
  not ok 1 - findWithOptions
    ---
    found: |-
      Array [
        Object {
          "unitDescription": "Created via upsert in integration test",
          "unitId": "<masked>",
          "unitName": "Widget Merged",
        },
        Object {
          "unitDescription": "First blong integration test widget",
          "unitId": "<masked>",
          "unitName": "Widget Alpha",
  ```


## blong-kopi

- 🔴 failed **$subject.play.ts › $Object › browse $subject $object** — `new`
  - trace: `traces/f82c454a-cf49-4014-9b1e-f857e8d9bbb0-attachment.zip`

## blong-kukum

- 🔴 failed **e2e.test.ts › the Playwright leg drives the model page against committed baselines › the Playwright suite exits 0** — `e2e.test.ts:285`

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
  # (node:27316) Warning: The 'NO_COLOR' env is ignored due to the 'FORCE_COLOR' env being set.
  # (Use `node --trace-warnings ...` to show where the warning was created)
  # (node:27607) Warning: The 'NO_COLOR' env is ignored due to the 'FORCE_COLOR' env being set.
  # (Use `node --trace-warnings ...` to show where the warning was created)
  # (node:27845) Warning: The 'NO_COLOR' env is ignored due to the 'FORCE_COLOR' env being set.
  # (Use `node --trace-warnings ...` to show where the warning was created)
  # (node:28564) Warning: The 'NO_COLOR' env is ignored due to the 'FORCE_COLOR' env being set.
  # (Use `node --trace-warnings ...` to show where the warning was created)
  # (node:28974) Warning: The 'NO_COLOR' env is ignored due to the 'FORCE_COLOR' env being set.
  # (Use `node --trace-warnings ...` to show where the warning was created)
  not ok 2 - the Playwright suite exits 0
    ---
    compare: ===
    at:
      fileName: e2e.test.ts
      lineNumber: 285
      columnNumber: 11
      typeName: Test
    stack: |
      Test.<anonymous> (e2e.test.ts:285:11)
    source: >2
                  t.comment(`Playwright exited ${status}. Last lines of its output:\n${tail}`);
              }
  ```


## blong-marine

- 🔴 failed **portal.play.ts › open and close browse tab** — `new`
  - trace: `traces/5ac75130-9607-4b42-b62d-82d776c3765d-attachment.zip`

## blong-suite

- 🔴 failed **../../../demo/blong-marine/test/portal.play.ts › open and close browse tab** — `new`
  - trace: `traces/47ea3597-e299-4593-b1d6-d294abbc5952-attachment.zip`

## blong-sport

- 🟡 flaky **relationships.play.ts › Relationships › edit sport specialist** — `new`
