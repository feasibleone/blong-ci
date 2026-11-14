# Failed tests

_feasibleone/blong · workflow Build · build #684_

[Full run](https://github.com/feasibleone/blong/actions/runs/43608145298) | [Allure report](index.html)

**2 failing test(s) in 2 package(s)**

## blong-gogo

- 🔴 failed **src/grant.test.ts › a grant asks for calls through the one seam the gateway uses › a short-lived token still verifies while it is live** — `src/grant.test.ts:167`

  The raw stream around it:

  ```tap
  # Subtest: an env key that is not a JWK is reported rather than used
  ok 1 - expected to reject
  ok 2 - verification refuses it too
  1..2
  ok 11 - an env key that is not a JWK is reported rather than used # time=7.088ms
  
  # Subtest: a grant asks for calls through the one seam the gateway uses
  ok 1 - a granted request asks for calls
  ok 2 - a request with no grant asks for nothing
  ok 3 - and a tampered one asks for nothing
  not ok 4 - a short-lived token still verifies while it is live
    ---
    at:
      fileName: src/grant.test.ts
      lineNumber: 167
      columnNumber: 7
      typeName: Test
    stack: |
      Test.<anonymous> (src/grant.test.ts:167:7)
    source: >2
          );
          const expired = await verifyGrant(await mintGrant({cap: ['calls'], ttlSeconds: 1}), undefined);
          t.ok((expired?.exp ?? 0) > 0, 'a short-lived token still verifies while it is live');
  ```


## blong-sport

- 🟡 flaky **reference.play.ts › Reference › create sport sport** — `new`
  - trace: `traces/22f72af6-4a47-4fc8-9259-08935abb1a5c-attachment.zip`
