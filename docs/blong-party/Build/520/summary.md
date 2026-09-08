### ❌ blong-party — 14 passed, 1 failed, 1 flaky (16 total)

| Status | Suite | Test | Trace |
| --- | --- | --- | --- |
| 🔴 failed | selfRegistration.play.ts | self-registration: create account and auto-login | `traces/ba3e7954-d718-42be-a3e4-4cfa43132d8e-attachment.zip` |
| 🟡 flaky | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal | `traces/b1f14675-a1f2-49d5-bbfd-51f006f9803d-attachment.zip` |

> **Traces**: Download the `playwright-traces` artifact and open `.zip` files at [trace.playwright.dev](https://trace.playwright.dev/)

<details><summary>All tests</summary>

| Status | Suite | Test |
| --- | --- | --- |
| 🔴 | selfRegistration.play.ts | self-registration: create account and auto-login |
| 🟡 | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal |
| 🟢 | organization.play.ts › Party Organization | browse party organization |
| 🟢 | organization.play.ts › Party Organization | create party organization |
| 🟢 | organization.play.ts › Party Organization | edit party organization |
| 🟢 | person.play.ts › Party Person | browse party person |
| 🟢 | person.play.ts › Party Person | create party person |
| 🟢 | person.play.ts › Party Person | edit party person |
| 🟢 | portal.play.ts | open and close organization browse tab |
| 🟢 | portal.play.ts | open and close person browse tab |
| 🟢 | portal.play.ts | portal loads after login |
| 🟢 | profile.play.ts › Party user profile | shows personal details and allows editing the profile and password |
| 🟢 | selfRegistration.play.ts | self-registration: password mismatch shows inline error |
| 🟢 | unit.play.ts › Party Unit | browse party unit |
| 🟢 | unit.play.ts › Party Unit | create party unit |
| 🟢 | unit.play.ts › Party Unit | edit party unit |

</details>

