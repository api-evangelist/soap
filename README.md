# SOAP (Simple Object Access Protocol)

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
