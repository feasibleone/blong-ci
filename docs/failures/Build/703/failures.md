# Failed tests

_feasibleone/blong · workflow Build · build #703_

[Full run](https://github.com/feasibleone/blong/actions/runs/44814694245) | [Allure report](index.html)

**2 failing test(s) in 2 package(s)**

## blong-agent

- 🔴 failed **test/lukaot.reach.test.ts › the declared signals reach the store, the service and the line › which is the tick the worker ran** — `test/lukaot.reach.test.ts:145`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,1 +1,1 @@
  -agent.worker.tick
  +test.agent.recovery
  ```


  The raw stream around it:

  ```tap
  ok 3 - and the line that announced it was printed
  ok 4 - the line carries a reference (2026-11-20T21:11:24.629Z info  dispatch flow=01M7XCSFK20Z8KF1VP4WVYVMZ1/-\#-1 leg=agent.worker.tick\#1 intent=test…
  ok 5 - the claim record carries the decision behind it
  ok 6 - and the arm that was taken
  ok 7 - and the intent names the entry that asked for the work, not the hop it was written on
  ok 8 - a session announces the loop that drives it
  ok 9 - and the mode it ran is a recorded decision
  ok 10 - and lukaot inspect resolves it against the store
  ok 11 - to the record the declared identifier names
  ok 12 - and the flow ledger lists the execution the claim belongs to
  not ok 13 - which is the tick the worker ran
    ---
    compare: ===
    at:
      fileName: test/lukaot.reach.test.ts
      lineNumber: 145
      columnNumber: 7
      typeName: Test
    stack: |
      Test.<anonymous> (test/lukaot.reach.test.ts:145:7)
    source: >2
          );
          t.ok(session, 'and the flow ledger lists the execution the claim belongs to');
  ```


## blong-sport

- 🟡 flaky **portal.play.ts › portal carries the sport menu** — `intermittent`
  - trace: `traces/6ceac109-a267-4e39-9207-5cfb4a8b4beb-attachment.zip`
