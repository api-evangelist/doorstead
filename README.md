# Doorstead

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Doorstead is a technology-enabled residential property management and tenant placement company
headquartered in San Francisco, serving single-family and small multifamily rental owners across
California, Washington, Florida, Texas, North Carolina, South Carolina, Ohio, Virginia and
Massachusetts. It sells two productized services — **Doorstead Place** (tenant placement only) and
**Doorstead Manage** (full-service property management). Doorstead discontinued its legacy Rent
Guarantee product in early 2025.

## API surface

**Doorstead publishes no public developer API.** There is no developer portal, API reference, SDK,
webhook catalog or machine-readable specification. `docs.doorstead.com`, `developer.doorstead.com`
and `developers.doorstead.com` do not resolve. The only API-shaped host, `api.doorstead.com`, is the
private GraphQL backend for Doorstead's own owner app and tenant portal; anonymous requests —
including GraphQL introspection — return `HTTP 403 {"message":"Unauthorized"}`.

What Doorstead *does* publish, and what this profile captures:

- [`llms/doorstead-llms.txt`](llms/doorstead-llms.txt) — a real, first-party `llms.txt` served at
  <https://www.doorstead.com/llms.txt>, saved verbatim
- [`plans/doorstead-plans-pricing.yml`](plans/doorstead-plans-pricing.yml) — the two published
  service plans and their fees (these are product plans, not API plans)
- [`security/doorstead-domain-security.yml`](security/doorstead-domain-security.yml) — probed
  TLS/DNSSEC/SPF/DMARC posture
- [`well-known/doorstead-well-known.yml`](well-known/doorstead-well-known.yml) — a recorded
  **absence**: every `/.well-known/` path 404s on every host that returns real status codes
- [`rate-limits/doorstead-rate-limits.yml`](rate-limits/doorstead-rate-limits.yml) — a recorded
  absence, `limit_count: 0`

## Links

- Website — <https://www.doorstead.com/>
- Pricing — <https://www.doorstead.com/compare-plans>
- Blog — <https://www.doorstead.com/blog>
- Knowledge base — <https://www.doorstead.com/knowledge>
- Tenant help — <https://tenants.doorstead.com/help>
- GitHub — <https://github.com/doorstead>
- Contact — <https://www.doorstead.com/contact-us>
