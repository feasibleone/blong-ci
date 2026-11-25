# Failed tests

_feasibleone/blong · workflow Build · build #719_

[Full run](https://github.com/feasibleone/blong/actions/runs/45705521262) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-int-adapter

- 🔴 failed **kafka.test.ts › blong int-adapter › kafka telemetry burst latency › burstsOfTraffic › throughput 132 msg/s is at least 150** — `../../core/blong-chain/executor.ts:469`

  ```
  simple
  ```


  The raw stream around it:

  ```tap
  | warm p95                       |  29.00 | ms      |
  | watch close                    |   1.00 | ms      |
  | sends over 100 ms              |   0.00 | sends   |
  | first send after silence (max) |  63.00 | ms      |
  | first after silence (max)      |  23.00 | ms      |
  
  2026-11-25T21:58:11.928Z error Watch flow=01M8ABEBQ78R1NK13J0HWZQEEH/kafka telemetry burst latency#0 intent=test.kafka.perf step burstsOfTraffic failed: th…
  step: burstsOfTraffic
  reason: throughput 132 msg/s is at least 150
  # Subtest: burstsOfTraffic
  not ok 1 - throughput 132 msg/s is at least 150
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

