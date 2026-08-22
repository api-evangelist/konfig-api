# Konfig (konfig-api)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Konfig is an SDK and API documentation generator that turns an OpenAPI Specification or Postman Collection into production-ready client libraries, interactive reference docs, demos, and tutorials. It generates and publishes idiomatic SDKs across TypeScript/JavaScript, Python, Java, C#, PHP, Ruby, Go, Swift, Kotlin, Objective-C, and Dart, republishing them automatically whenever the spec changes, and layers on OpenAPI linting and generated SDK tests to keep client libraries in sync across the API lifecycle.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/konfig-api/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/konfig-api/refs/heads/main/apis.yml)

## Access Model (Read This First)

Konfig is a **developer-tooling platform, not a hosted public REST API**. There is no documented public base URL, endpoint list, or authentication scheme for third-party programmatic access. Publishers use Konfig through:

- **`konfig-cli`** (npm: `konfig-cli`, Node 14+) — commands `konfig init`, `konfig generate`, `konfig test`, `konfig publish`.
- **`konfig.yaml`** — a declarative config with a `generators` block (spec path, output directories, per-language SDK settings).
- A **web dashboard / interactive tutorial** and **GitHub integration**.

`konfig generate` calls Konfig's hosted generator backend, but that backend is internal and undocumented — it is not a versioned public API. Because of this, the product surfaces in `apis.yml` are recorded as **`endpointsModeled` capability areas** (SDK Generation, SDK Publishing, Documentation Portal, Demos & Tutorials, OpenAPI Linting) rather than real REST endpoints. No OpenAPI or collection artifact was fabricated.

## Company Status

Konfig was a developer-tools startup founded in 2022 in Los Angeles by Anh-Tuan Bui and Dylan Huang. It was **sunset as of December 2024**, and its full codebase was **open-sourced under the MIT license** at [github.com/konfig-dev/konfig](https://github.com/konfig-dev/konfig). The marketing site ([konfigthis.com](https://konfigthis.com)), the documentation, and the **491 generated SDK repositories** at [github.com/konfig-sdks](https://github.com/konfig-sdks) remain online and self-hostable. There is no active commercial offering as of this writing — the live path is self-hosting the open-source generator.

## Tags

- SDK Generation
- Client Library
- API Documentation
- Developer Tools
- API Lifecycle
- OpenAPI
- Code Generation

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs (Capability Areas — endpointsModeled)

### Konfig SDK Generation

Generates idiomatic client-library SDKs from an OpenAPI Specification or Postman Collection in TypeScript/JavaScript, Python, Java, C#, PHP, Ruby, Go, Swift, Kotlin, Objective-C, and Dart. Driven by `konfig init` / `konfig generate` reading the `konfig.yaml` generators block.

- **Human URL:** [https://konfigthis.com/docs/getting-started/](https://konfigthis.com/docs/getting-started/)

#### Tags

- SDK Generation
- Client Library
- Code Generation
- OpenAPI

#### Properties

- [Documentation](https://konfigthis.com/docs/)
- [konfig.yaml Reference](https://konfigthis.com/docs/konfig-yaml/)
- [konfig-cli (npm)](https://www.npmjs.com/package/konfig-cli)

### Konfig SDK Publishing and Updates

Tests and publishes generated SDKs to package registries (npm, PyPI, Maven Central/Sonatype, and others) via `konfig test` and `konfig publish`, and automatically republishes every SDK when the source spec changes. Published SDK repositories live under [github.com/konfig-sdks](https://github.com/konfig-sdks).

- **Human URL:** [https://konfigthis.com/docs/tutorials/automate-sdk-updates/](https://konfigthis.com/docs/tutorials/automate-sdk-updates/)

#### Tags

- Client Library
- Publishing
- API Lifecycle
- Package Managers

### Konfig Documentation Portal

Generates branded, interactive API reference documentation and markdown pages from the same OpenAPI spec, embedding language-specific SDK snippets that auto-update whenever the spec is republished.

- **Human URL:** [https://konfigthis.com/docs/](https://konfigthis.com/docs/)

#### Tags

- API Documentation
- Developer Portal
- Reference Docs

### Konfig Demos and Tutorials

Builds interactive, runnable demos and markdown-based tutorials on top of the generated SDKs so API consumers can onboard and try live calls from the developer portal.

- **Human URL:** [https://konfigthis.com/interactive-tutorial/](https://konfigthis.com/interactive-tutorial/)

#### Tags

- Developer Tools
- Demos
- Tutorials
- Onboarding

### Konfig OpenAPI Linting

A configurable linter that inspects an OpenAPI Specification for errors and quality issues before SDK and docs generation, so client libraries are produced from a clean, consistent spec.

- **Human URL:** [https://konfigthis.com/docs/lint-rules/](https://konfigthis.com/docs/lint-rules/)

#### Tags

- Linting
- API Governance
- OpenAPI
- Developer Tools

## Common Properties

- [GitHub Organization](https://github.com/konfig-dev)
- [Generated SDKs (github.com/konfig-sdks)](https://github.com/konfig-sdks)
- [LinkedIn](https://www.linkedin.com/company/konfig)
- [Website](https://konfigthis.com)
- [Documentation](https://konfigthis.com/docs)
- [Plans](plans/konfig-api-plans-pricing.yml)
- [Rate Limits](rate-limits/konfig-api-rate-limits.yml)
- [Fin Ops](finops/konfig-api-finops.yml)
- [Blog](https://konfigthis.com/blog)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
