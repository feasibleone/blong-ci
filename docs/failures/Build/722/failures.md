# Failed tests

_feasibleone/blong · workflow Build · build #722_

[Full run](https://github.com/feasibleone/blong/actions/runs/45841955469) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-int-adapter

- 🔴 failed **kafka.test.ts › blong int-adapter › kafka telemetry burst latency › burstsOfTraffic › throughput 129 msg/s is at least 150** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  | warm p95                       |  23.00 | ms      |
  | watch close                    |   0.00 | ms      |
  | sends over 100 ms              |   1.00 | sends   |
  | first send after silence (max) | 114.00 | ms      |
  | first after silence (max)      |  14.00 | ms      |
  
  2026-11-26T15:09:07.880Z error Watch flow=01M8C6E1KBTW1C1WYMWG4P289Q/kafka telemetry burst latency#0 intent=test.kafka.perf step burstsOfTraffic failed: th…
  step: burstsOfTraffic
  reason: throughput 129 msg/s is at least 150
  # Subtest: burstsOfTraffic
  not ok 1 - throughput 129 msg/s is at least 150
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

