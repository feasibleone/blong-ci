# Failed tests

_feasibleone/blong · workflow Build · build #721_

[Full run](https://github.com/feasibleone/blong/actions/runs/45832653933) | [Allure report](index.html)

**3 failing test(s) in 3 package(s)**

## blong-agent

- 🔴 failed **index.test.ts › timeout!** — `index.test.ts`

  ```
  timeout: the run's own budget expired while this test was still running
  ```


  The raw stream around it:

  ```tap
  2026-11-26T14:22:12.595Z info  agent.agentDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8C3RH3K6Q7GHDWTPAES48BW]
    writeDropped: 163
  2026-11-26T14:22:12.596Z info  agent.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8C3RH3K6Q7GHDWTPAES48BX]
    writeDropped: 163
  2026-11-26T14:22:12.596Z info  gateway.meter(redis) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8C3RH3MQC09YAEE0SNX4X3C]
    writeDropped: 163
  2026-11-26T14:22:12.598Z info  gateway.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8C3RH3MQC09YAEE0SNX4X3D]
    writeDropped: 163
  2026-11-26T14:22:12.598Z info  testRealm.testDispatch(dispatch) event adapter.stop [lukaot://t/0cc3bf136c8a p=01M8C3RH3PBTDS7A69M1RA9A37]
    writeDropped: 163
  not ok 2 - timeout!
    ---
    signal: SIGALRM
    expired: TAP
    test: TAP
    ...
  
  1..2
  # time=240018.219ms
  not ok 1 - index.test.ts # time=240018.219ms
  ---
  stdio: pipe
  cwd: /home/runner/work/blong/blong/realm/blong-agent
  ```


## blong-int-adapter

- 🔴 failed **kafka.test.ts › blong int-adapter › kafka telemetry burst latency › burstsOfTraffic › throughput 131 msg/s is at least 150** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  | warm p95                       |  21.00 | ms      |
  | watch close                    |   0.00 | ms      |
  | sends over 100 ms              |   0.00 | sends   |
  | first send after silence (max) |  85.00 | ms      |
  | first after silence (max)      |   9.00 | ms      |
  
  2026-11-26T14:14:22.579Z error Watch flow=01M8C39SKH24WVBFA99HC9V5JM/kafka telemetry burst latency#0 intent=test.kafka.perf step burstsOfTraffic failed: th…
  step: burstsOfTraffic
  reason: throughput 131 msg/s is at least 150
  # Subtest: burstsOfTraffic
  not ok 1 - throughput 131 msg/s is at least 150
    ---
    stack: |
      call (../../core/blong-chain/executor.ts:469:28)
      Proxy.<anonymous> (../../core/blong-chain/executor.ts:498:44)
      burstsOfTraffic (kafka/test/test/testKafkaPerf.ts:327:32)
      executeStepFn (../../core/blong-chain/executor.ts:1005:34)
      Test.<anonymous> (../../core/blong-chain/executor.ts:1174:17)
    at:
      fileName: ../../core/blong-chain/executor.ts
      lineNumber: 469
      columnNumber: 28
      functionName: call
  ```


## blong-sport

- 🟡 flaky **portal.play.ts › portal carries the sport menu** — `new`
  - trace: `traces/66b12bdf-784f-47e6-a43b-ba25f6de8d02-attachment.zip`
