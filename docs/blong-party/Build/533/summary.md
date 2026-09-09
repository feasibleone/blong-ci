### ❌ blong-party — 14 passed, 1 failed, 1 flaky (16 total)

| Status | Suite | Test | Trace |
| --- | --- | --- | --- |
| 🔴 failed | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal | `traces/6aaf4010-1a1a-4d8d-9dfc-f12f8e140596-attachment.zip` |
| 🟡 flaky | profile.play.ts › Party user profile | shows personal details and allows editing the profile and password | `traces/7de50ca6-f702-48be-9e3d-babdc4d84a80-attachment.zip` |

> **Traces**: Download the `playwright-traces` artifact and open `.zip` files at [trace.playwright.dev](https://trace.playwright.dev/)

<details><summary>All tests</summary>

| Status | Suite | Test |
| --- | --- | --- |
| 🔴 | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal |
| 🟡 | profile.play.ts › Party user profile | shows personal details and allows editing the profile and password |
| 🟢 | organization.play.ts › Party Organization | browse party organization |
| 🟢 | organization.play.ts › Party Organization | create party organization |
| 🟢 | organization.play.ts › Party Organization | edit party organization |
| 🟢 | person.play.ts › Party Person | browse party person |
| 🟢 | person.play.ts › Party Person | create party person |
| 🟢 | person.play.ts › Party Person | edit party person |
| 🟢 | portal.play.ts | open and close organization browse tab |
| 🟢 | portal.play.ts | open and close person browse tab |
| 🟢 | portal.play.ts | portal loads after login |
| 🟢 | selfRegistration.play.ts | self-registration: create account and auto-login |
| 🟢 | selfRegistration.play.ts | self-registration: password mismatch shows inline error |
| 🟢 | unit.play.ts › Party Unit | browse party unit |
| 🟢 | unit.play.ts › Party Unit | create party unit |
| 🟢 | unit.play.ts › Party Unit | edit party unit |

</details>

