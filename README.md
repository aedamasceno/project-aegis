# Project AEGIS

**Free, open-source, privacy-first AI assistance for law enforcement and public safety.**

**Status:** Planning / pre-prototype. This repository documents a proposed project. No operational software or agency deployment is available yet.

## Mission

Project AEGIS aims to help public safety agencies—especially smaller departments with limited technical budgets—benefit from locally hosted AI tools without mandatory cloud services or software licensing fees.

The project is an independent open-source effort led by [Emanuel Damasceno](https://github.com/aedamasceno), a law enforcement professional and Cisco CCIE Collaboration engineer (#40965).

## Initial project areas

- **Incident documentation assistance:** Organize officer-provided notes into structured drafts, flag missing details, and preserve clear separation between source facts and AI suggestions.
- **Citation-grounded reference retrieval:** Retrieve statutes, agency-approved policies, and training references with source links, dates, and review prompts.
- **Scenario-based training:** Develop synthetic training exercises for communication, crisis response, and decision-making practice.
- **Local AI deployment:** Evaluate private, on-premises inference using Linux and locally hosted language models.

These are proposed capabilities, **not currently available features**.

## Guiding principles

- Free and open-source software, with publicly accessible code and documentation.
- Local processing by default; no mandatory external AI processing.
- Human review of all generated content and operational decisions.
- No autonomous arrest, detention, use-of-force, suspect identification, or individual risk-scoring decisions.
- No invented facts or unsupported legal citations presented as authoritative.
- Strong access control, auditability, data minimization, and testability.
- Synthetic data for public examples and development unless other data is explicitly authorized and appropriately protected.

## Proposed technical architecture

```text
Browser / local UI
        |
Application API and authentication
        |
+-----------------------------+
| Document assistance         |
| Reference search / RAG      |
| Training scenario generator |
+-----------------------------+
        |
Local model inference + source storage
        |
Linux / NVIDIA GPU or other supported hardware
```

The architecture is exploratory and will evolve as prototypes are implemented and tested.

## Development roadmap

See [docs/ROADMAP.md](docs/ROADMAP.md). The first milestone is a local, synthetic-data-only report-assistance prototype with source attribution, review controls, and repeatable evaluations.

## Hardware research

Existing NVIDIA RTX 4090 and RTX 3090 hardware can support baseline experiments. A proposed NVIDIA DGX Spark evaluation would investigate larger-memory model workloads and compare latency, throughput, quality, power use, and deployment constraints. **No NVIDIA sponsorship or endorsement is claimed.**

The eventual software should support practical, affordable deployment wherever technically feasible. DGX Spark is a proposed development system, not a requirement for agencies.

## Safety and privacy

This project is not an emergency response tool, a substitute for legal counsel, or an autonomous law-enforcement decision system. All outputs must be verified by qualified personnel. See [SECURITY.md](SECURITY.md) for responsible disclosure and data-handling expectations.

## Contributing

The project welcomes technical review, design feedback, documentation contributions, and eventually code contributions. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Apache License 2.0. See [LICENSE](LICENSE).
