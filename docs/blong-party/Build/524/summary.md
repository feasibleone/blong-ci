### ⚠️ blong-party — 14 passed, 0 failed, 2 flaky (16 total)

| Status | Suite | Test | Trace |
| --- | --- | --- | --- |
| 🟡 flaky | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal | `traces/232d3345-908f-442a-86c7-9d95afd7fa54-attachment.zip` |
| 🟡 flaky | profile.play.ts › Party user profile | shows personal details and allows editing the profile and password | `traces/60ec5c53-b86c-45f5-afae-8b4f1fa13f4c-attachment.zip` |

> **Traces**: Download the `playwright-traces` artifact and open `.zip` files at [trace.playwright.dev](https://trace.playwright.dev/)

<details><summary>All tests</summary>

| Status | Suite | Test |
| --- | --- | --- |
| 🟡 | googleLogin.play.ts | google login (mock) auto-registers and lands in the portal |
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

