# Failed tests

_feasibleone/blong · workflow Build · build #643_

[Full run](https://github.com/feasibleone/blong/actions/runs/40598911517) | [Allure report](index.html)

**5 failing test(s) in 1 package(s)**

## blong-kustomize

- 🔴 failed **index.test.ts › kustomize flow (server) › plan find › planIsDeterministic › plan** — `../../core/blong-chain/executor.ts:917`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -75,21 +75,21 @@
         },
       ],
       "suite": Object {
         "database": false,
         "entry": undefined,
         "frameworkImage": "ghcr.io/feasibleone/blong-gogo",
         "intents": undefined,
         "minFrameworkVersion": undefined,
         "name": "blong-suite",
         "namespace": "blong-suite",
  -      "version": "0.1.0",
  +      "version": "0.2.0",
       },
       "suiteVolume": Object {
         "artifact": undefined,
         "attemptRetention": 5,
         "backend": "nodeLocal",
         "retention": 3,
         "rwxManifest": undefined,
         "rwxProvider": undefined,
         "storageClassName": undefined,
       },
  ```


  The raw stream around it:

  ```tap
  # Subtest: aRealmDeclaresItsOwnRole
  1..0
  ok 2 - aRealmDeclaresItsOwnRole # time=14.94ms
  
  # Subtest: theOperatorIsAnotherTree
  1..0
  ok 3 - theOperatorIsAnotherTree # time=8.258ms
  
  # Subtest: planIsDeterministic
  not ok 1 - plan
    ---
    found: |-
      Object {
        "assets": Array [],
        "backingServiceRequest": Object {},
        "backingServices": Array [],
        "crd": undefined,
        "deployments": Array [
          Object {
            "layers": Array [
              "kustomize.orchestrator",
              "kustomize.gateway",
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › aSplitTreeKeepsTheArtifactOutOfTheBase › splitTree** — `../../core/blong-chain/executor.ts:917`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -7,22 +7,22 @@
         "name: blong",
       ],
       "fillImageInTemplate": true,
       "frameworkImageInBase": false,
       "frameworkImageInOverlay": true,
       "identityInBase": false,
       "identityInBaseFiles": Array [],
       "identityInLocal": true,
       "imagesInBase": 2,
       "instanceDirs": Array [
  -      "local/suite/cache/blong-suite-fill-0.1.0-a1b2c3d4-node-a",
  -      "local/suite/cache/blong-suite-fill-0.1.0-a1b2c3d4-node-b",
  +      "local/suite/cache/blong-suite-fill-0.2.0-a1b2c3d4-node-a",
  +      "local/suite/cache/blong-suite-fill-0.2.0-a1b2c3d4-node-b",
       ],
       "moduleInBase": false,
       "namespacesInBase": 0,
       "nodesInBase": 0,
       "nodesInLocal": 2,
       "patches": 13,
       "placeholderInBase": true,
       "placeholdersInTemplate": true,
       "realVolumeInPatch": true,
       "rootNamesNamespace": false,
  ```


  The raw stream around it:

  ```tap
  # Subtest: theSerializedTreeIgnoresKeyOrder
  1..0
  ok 2 - theSerializedTreeIgnoresKeyOrder # time=55.132ms
  
  # Subtest: aCrSpecDrivesTheTree
  ok 1 - crSpec
  1..1
  ok 3 - aCrSpecDrivesTheTree # time=28.932ms
  
  # Subtest: aSplitTreeKeepsTheArtifactOutOfTheBase
  not ok 1 - splitTree
    ---
    found: |-
      Object {
        "deploymentPatch": Array [
          "- image: ghcr.io/feasibleone/blong-gogo:latest",
          "app.kubernetes.io/name: blong-suite",
          "app.kubernetes.io/name: blong-suite",
          "name: blong",
        ],
        "fillImageInTemplate": true,
        "frameworkImageInBase": false,
        "frameworkImageInOverlay": true,
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › theOperatorIsInstalledOnceForTheCluster › operatorInstall** — `../../core/blong-chain/executor.ts:917`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,22 +1,22 @@
   String(
     Object {
       "addressedIngress": Object {
         "apiVersion": "networking.k8s.io/v1",
         "kind": "Ingress",
         "metadata": Object {
           "labels": Object {
             "app.kubernetes.io/managed-by": "blong-kustomize",
             "app.kubernetes.io/name": "blong-operator",
             "app.kubernetes.io/part-of": "blong-operator",
  -          "app.kubernetes.io/version": "0.1.0",
  -          "blong.feasible.one/spec-hash": "acdfe2e9caec044f",
  +          "app.kubernetes.io/version": "0.2.0",
  +          "blong.feasible.one/spec-hash": "37e56d0891fbf0cf",
           },
           "name": "blong-operator-test",
           "namespace": "blong-system",
         },
         "spec": Object {
           "rules": Array [
             Object {
               "host": "blong-operator.test",
               "http": Object {
                 "paths": Array [
  @@ -47,22 +47,22 @@
         ],
         Array [
           "subjectaccessreviews",
           Array [
             "create",
           ],
         ],
       ],
       "installFiles": Array [
         "cache/kustomization.yaml",
  -      "cache/shop-fill-0.1.0-node-a.yaml",
  -      "cache/shop-fill-
  ```


  The raw stream around it:

  ```tap
  source: |2
          let started = false;
          try {
              await scope.test(name, async (sub: unknown) => {
  ------------------------^
                  started = true;
                  await run(sub as ITestFrameworkContext);
  ...
  
  # Subtest: theOperatorIsInstalledOnceForTheCluster
  not ok 1 - operatorInstall
    ---
    found: |-
      Object {
        "addressedIngress": Object {
          "apiVersion": "networking.k8s.io/v1",
          "kind": "Ingress",
          "metadata": Object {
            "labels": Object {
              "app.kubernetes.io/managed-by": "blong-kustomize",
              "app.kubernetes.io/name": "blong-operator",
              "app.kubernetes.io/part-of": "blong-operator",
              "app.kubernetes.io/version": "0.2.0",
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › theTreeCarriesWhatARealmDeclares › realmDeclarations** — `../../core/blong-chain/executor.ts:917`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,20 +1,20 @@
   String(
     Object {
       "generatedFolders": Array [
         "assets/kustomization.yaml",
         "secrets/kustomization.yaml",
       ],
       "mounted": Array [
         Object {
           "hostPath": Object {
  -          "path": "/var/lib/blong/suites/shop/0.1.0",
  +          "path": "/var/lib/blong/suites/shop/0.2.0",
             "type": "Directory",
           },
           "name": "suite",
         },
         Object {
           "name": "shop-data",
           "persistentVolumeClaim": Object {
             "claimName": "shop-data",
           },
         },
  ```


  The raw stream around it:

  ```tap
  1..1
  ok 32 - aVolumeIsNamedAfterItsArtifact # time=2.202ms
  
  # Subtest: objectsAreFingerprinted
  ok 1 - generatedFileCount
  ok 2 - generatedTree
  1..2
  ok 33 - objectsAreFingerprinted # time=6.798ms
  
  # Subtest: theTreeCarriesWhatARealmDeclares
  not ok 1 - realmDeclarations
    ---
    found: |-
      Object {
        "generatedFolders": Array [
          "assets/kustomization.yaml",
          "secrets/kustomization.yaml",
        ],
        "mounted": Array [
          Object {
            "hostPath": Object {
              "path": "/var/lib/blong/suites/shop/0.2.0",
              "type": "Directory",
  ```

- 🔴 failed **index.test.ts › kustomize flow (server) › tree generate › theVersionLabelIsTheSuitesOwn › versionLabels** — `../../core/blong-chain/executor.ts:917`

  ```
  assertion failed (===)
  --- expected
  +++ actual
  @@ -1,7 +1,7 @@
   String(
     Object {
       "declared": "9.8.7",
  -    "realm": "0.1.0",
  -    "unversioned": "0.1.0",
  +    "realm": "0.2.0",
  +    "unversioned": "0.2.0",
     }
   )
  ```


  The raw stream around it:

  ```tap
  ok 2 - migrationStep
  1..2
  ok 29 - everyNamespaceTheResolverAsksForHasAService # time=5.98ms
  
  # Subtest: everyReferenceInTheTreeResolves
  ok 1 - danglingReferences
  1..1
  ok 30 - everyReferenceInTheTreeResolves # time=5.731ms
  
  # Subtest: theVersionLabelIsTheSuitesOwn
  not ok 1 - versionLabels
    ---
    found: |-
      Object {
        "declared": "9.8.7",
        "realm": "0.2.0",
        "unversioned": "0.2.0",
      }
    wanted: |-
      Object {
        "declared": "9.8.7",
        "realm": "0.1.0",
        "unversioned": "0.1.0",
  ```

