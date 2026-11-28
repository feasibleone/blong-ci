# Failed tests

_feasibleone/blong · workflow Build · build #725_

[Full run](https://github.com/feasibleone/blong/actions/runs/46143994064) | [Allure report](index.html)

**4 failing test(s) in 3 package(s)**

## blong-agent

- 🔴 failed **index.test.ts › timeout!** — `index.test.ts`

  ```
  timeout: the run's own budget expired while this test was still running
  ```


  The raw stream around it:

  ```tap
  2026-11-28T12:49:31.220Z info  agent.engine(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882MKG7T6WC25646GDRY]
  2026-11-28T12:49:31.221Z info  agent.kafka(kafka) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882MKG7T6WC25646GDRZ]
  2026-11-28T12:49:31.224Z info  agent.notify(redis) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882NT4P62NXNB78Z2EFJ]
  2026-11-28T12:49:31.224Z info  agent.task(http) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882RZYVM2SZRRKP6EGC7]
  2026-11-28T12:49:31.224Z info  agent.workspace(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882RZYVM2SZRRKP6EGC8]
  2026-11-28T12:49:31.225Z info  agent.agentDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882RZYVM2SZRRKP6EGC9]
  2026-11-28T12:49:31.225Z info  agent.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882S69S7PN9J1G4BMQPM]
  2026-11-28T12:49:31.225Z info  gateway.meter(redis) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882S69S7PN9J1G4BMQPN]
  2026-11-28T12:49:31.225Z info  gateway.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882S69S7PN9J1G4BMQPP]
  2026-11-28T12:49:31.225Z info  testRealm.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8H3882S69S7PN9J1G4BMQPQ]
  not ok 2 - timeout!
    ---
    signal: SIGALRM
    expired: TAP
    test: TAP
    ...
  
  1..2
  # time=240022.882ms
  not ok 1 - index.test.ts # time=240022.882ms
  ---
  stdio: pipe
  cwd: /home/runner/work/blong/blong/realm/blong-agent
  ```


## blong-commander

- 🔴 failed **explore.play.ts › kafka-dev — topics and message viewer** — `new`
  - trace: `traces/9ade7c2d-27e9-4bce-a34f-d7e75dc427d7-attachment.zip`

## blong-sport

- 🟡 flaky **reference.play.ts › Reference › edit sport discipline** — `new`
  - trace: `traces/de30d8ce-3702-4601-a2e0-bd867017d88e-attachment.zip`
- 🟡 flaky **portal.play.ts › portal carries the sport menu** — `new`
  - trace: `traces/1220924b-d87b-4de2-b336-8e62a29f5e73-attachment.zip`
