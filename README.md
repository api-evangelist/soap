# SOAP (Simple Object Access Protocol)

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

SOAP (Simple Object Access Protocol) is an XML-based messaging protocol for exchanging structured information in web services, standardized by W3C as SOAP 1.2 (Second Edition, 2007). It provides a platform-independent, language-neutral framework for web service communication with built-in standards for security (WS-Security), reliable messaging, and transactions.

## Specification

- **SOAP 1.2 Part 1 (Messaging Framework):** https://www.w3.org/TR/soap12-part1/
- **SOAP 1.2 Part 2 (Adjuncts/HTTP Binding):** https://www.w3.org/TR/soap12-part2/
- **SOAP 1.1 Note (2000):** https://www.w3.org/TR/2000/NOTE-SOAP-20000508/
- **W3C XML Protocol Working Group:** https://www.w3.org/2000/xp/Group/

## Message Structure

A SOAP message consists of:
- **Envelope** — root element wrapping the entire message
- **Header** (optional) — metadata and processing directives for SOAP nodes
- **Body** (required) — the main payload for the ultimate receiver
- **Fault** — error reporting structure within the Body

## Fault Codes

| Code | Description |
|------|-------------|
| VersionMismatch | Unknown SOAP envelope namespace |
| MustUnderstand | Required header block not processed |
| DataEncodingUnknown | Unknown encoding style |
| Sender | Message error caused by the sender |
| Receiver | Processing failure at the receiver |

## Artifacts

| Type | File |
|------|------|
| JSON Schema (Envelope) | [json-schema/soap-envelope.json](json-schema/soap-envelope.json) |
| JSON Schema (Header) | [json-schema/soap-header.json](json-schema/soap-header.json) |
| JSON Schema (Header Block) | [json-schema/soap-header-block.json](json-schema/soap-header-block.json) |
| JSON Schema (Body) | [json-schema/soap-body.json](json-schema/soap-body.json) |
| JSON Schema (Fault) | [json-schema/soap-fault.json](json-schema/soap-fault.json) |
| JSON-LD Context | [json-ld/soap-context.jsonld](json-ld/soap-context.jsonld) |
| JSON Structure | [json-structure/soap-envelope-structure.json](json-structure/soap-envelope-structure.json) |
| Vocabulary | [vocabulary/soap-vocabulary.yml](vocabulary/soap-vocabulary.yml) |
| Examples | [examples/soap-envelope-example.json](examples/soap-envelope-example.json) |

## Timestamps

- **Created:** 2025
- **Modified:** 2026-05-02
