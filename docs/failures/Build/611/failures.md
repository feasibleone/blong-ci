# Failed tests

_feasibleone/blong · workflow Build · build #611_

[Full run](https://github.com/feasibleone/blong/actions/runs/38426185641) | [Allure report](index.html)

**1 failing test(s) in 1 package(s)**

## blong-kustomize

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › objectsAreFingerprinted › generatedTree** — `../../core/blong-chain/index.ts:780`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -146,29 +146,29 @@
         apiVersion: kustomize.config.k8s.io/v1beta1
         kind: Kustomization
         resources:
           - blong-suite-fill-1.0.0-node-a.yaml
           - blong-suite-fill-1.0.0-node-b.yaml
  
       ),
       "configmaps/fill-script.yaml": String(
         apiVersion: v1
         binaryData:
  -        fill.mts: LyoqCiAqIGZpbGwudHMg4oCUIGJyaW5nIGEgc3VpdGUgYXJ0aWZhY3QgdG8gd2hlcmUgaXQgaXMgcmVhZCBmcm9tLCBhcyBvbmUgcHJvZ3JhbSB3aXRoIHR3byBjYWxsZXJzLgogKgogKiBUaGUgb3BlcmF0b3IgZmV0Y2hlcyBhbiBhcnRpZmFjdCBpbnRvIGl0cyBvd24gY2FjaGUgd2hpbGUgaXQgcGxhbnMsIGFuZCBhIG5vZGUncyBmaWxsIEpvYiBzdGFnZXMgb25lCiAqIGJlc2lkZSB0aGUgZGlyZWN0b3J5IGl0IHdpbGwgb2NjdXB5IGFuZCByZW5hbWVzIGl0IGludG8gcGxhY2UuIFRoZXkgbXVzdCBhZ3JlZSBhYm91dCB3aGF0IGFuIGFydGlmYWN0CiAqIGlzIGFuZCB3aGF0IG1ha2VzIGl0IHdob2xlLCBzbyB0aGUgcGllY2VzIOKAlCBmZXRjaCwgdW5wYWNrLCBsaW5rLCBtYWtlIHBvcnRhYmxlLCBtYXJrLCByZXRhaW4g4oCUIGFyZQogKiBkZWZpbmVkIG9uY2UgaGVyZSBhbmQgZGlmZmVyIG9ubHkgaW4gd2hhdCBhIGNhbGxlciBwYXNzZXMuIFRoZSBzYW1lIGZpbGUgaXMgd2hhdCB0aGUgY29udGFpbmVyIHJ1bnM6CiAqIGl0IGlzIG1vdW50ZWQgaW50byB0aGUgZmlsbCBKb2IgYW5kIHN0YXJ0ZWQgd2l0aCBgbm9kZWAsIHdoaWNoIGlzIHRoZSB3aG9sZSByZWFzb24gdGhpcyBpcyBhIG1vZH
  ```

