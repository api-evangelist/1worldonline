# 1World Online

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

1World Online is an audience-engagement and interactive-advertising company, operating since 2012,
that serves media publishers, advertisers and travel brands. Its platform embeds Interactive Media
Units — polls, quizzes, trivia, debates and surveys — into publisher pages in 30+ languages, turns
the resulting engagement into interactive ad inventory and first-party audience insight, and rewards
participants through a points-based loyalty program and Web3 collectables (TravelVerse). It also
operates a technology center offering custom development and integration services.

## API surface

**There is a live API. There is no published contract.**

- The platform backend is live at `https://app-wleu.1worldonline.com/`. 1World Online's own frontend
  configuration names it (`URL_SERVER_API_NEW`), and the host serves a Spring Boot Actuator index
  whose self href names the same host — which is how first-party ownership was established.
- No developer portal, API reference, OpenAPI, Swagger, GraphQL SDL, AsyncAPI, WSDL, Postman
  collection, MCP server or A2A agent card is published anywhere. Every conventional specification
  path on the API host and both website hosts returns 404, and `POST /graphql` returns 404.
- No `/.well-known/` document is served on any host. Two hosts (`frontend-wleu`, `portal-wleu`) are
  single-page-app catch-alls that answer 200 with an HTML shell for every path including a
  negative-control path that cannot exist, so their 200s were discarded rather than recorded as hits.
- A public Swagger UI for a 1World Online Polls API was once served at `http://api.1worldonline.com/`.
  That host no longer resolves in DNS. Nothing from the archive was republished here as a contract.
- Access runs through publisher/advertiser partner registration, not a self-serve developer key.

## Artifacts

| Path | What it records |
|---|---|
| `apis.yml` | APIs.json index — identity, links, and the one platform API entry |
| `lifecycle/` | Versioning, the open Actuator health endpoint, and the retired public API host |
| `plans/` | No published plans — recorded zero, with quotes from the provider's own pages |
| `rate-limits/` | No published limits — recorded zero |
| `packages/` | No first-party SDK — npm, PyPI and both GitHub accounts probed |
| `mcp/` | No MCP server — `deployment.mode: none` |
| `well-known/` | Full `/.well-known` probe record across six hosts, with soft-404 controls |
| `security/` | TLS / HSTS / DNSSEC / CAA / SPF / DMARC probe |
| `llms/` | Generated `llms.txt` (1World Online publishes none) |

Links: https://1worldonline.com/ · https://welcome.1worldonline.com/ · https://github.com/1worldonline-rnd
