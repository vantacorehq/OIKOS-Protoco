<p align="center">
  <img src="banner.svg" alt="OIKOS Protocol" width="100%">
</p>

<p align="center">
  <b>English</b> · <a href="README.ru.md">Русский</a>
</p>

<p align="center">
  <img alt="status" src="https://img.shields.io/badge/status-concept%20%2F%20RFC-D4B26F?style=flat-square&labelColor=0E1A44">
  <img alt="license" src="https://img.shields.io/badge/license-AGPL--3.0-EAF0FF?style=flat-square&labelColor=0E1A44">
  <img alt="governance" src="https://img.shields.io/badge/governance-open-5F73A8?style=flat-square&labelColor=0E1A44">
  <img alt="PRs" src="https://img.shields.io/badge/PRs-welcome-D4B26F?style=flat-square&labelColor=0E1A44">
</p>

# OIKOS Protocol

**A global, decentralized system for automatic allocation of planetary resources, built on open AI.**

OIKOS (Greek *oikos*, "household" — the root of the word *economy*) is an open-source protocol for
measuring, modelling and allocating the resources of a single shared planet: food, water, energy,
materials, medicine and compute. It is designed to operate without dependence on national borders,
administrative bottlenecks, or patent barriers on essential medicines.

> **Status:** concept and request for comments. This repository defines the vision, architecture and
> research agenda. Nothing here is deployed, and nothing should be treated as a finished system.

---

## Why

- Resources are produced in one place and needed in another, but the data that would connect the two is fragmented, closed and slow.
- Allocation decisions are made behind opaque processes that cannot be audited by the people they affect.
- Life-saving knowledge — including essential medicine — is gated by patents, not by the ability to produce it.

OIKOS asks one question: **what if allocation were transparent, computable and verifiable by anyone?**

## Principles

| Principle | Meaning |
|---|---|
| **Open by default** | Code, models, weights, data schemas and decision logs are public. |
| **Verifiable** | Every allocation is reproducible from public inputs. No black boxes. |
| **Decentralized** | No single operator, jurisdiction or key can control or shut down the network. |
| **Borderless** | Allocation is computed on need and capacity, not on administrative geography. |
| **Human sovereignty** | AI proposes; people can inspect, contest and override through open governance. |
| **Do no harm** | Hard constraints and safety review precede any capability. |

## Architecture

```
┌──────────────────────────────────────────────────────────┐
│  5  Governance      open proposals · voting · overrides  │
├──────────────────────────────────────────────────────────┤
│  4  Allocation      open-model planners · optimizers     │
├──────────────────────────────────────────────────────────┤
│  3  Ledger          decentralized, append-only, auditable│
├──────────────────────────────────────────────────────────┤
│  2  Resource Graph  supply · demand · logistics · stock  │
├──────────────────────────────────────────────────────────┤
│  1  Sensing         open data feeds · attestations       │
└──────────────────────────────────────────────────────────┘
```

1. **Sensing** — ingest open and attested data on production, stock, demand and transport.
2. **Resource Graph** — a shared, versioned model of the planet's flows.
3. **Ledger** — tamper-evident record of inputs, decisions and outcomes.
4. **Allocation** — open models that propose distributions under explicit, published objectives and constraints.
5. **Governance** — the layer where people set objectives, review decisions and revoke authority.

## Roadmap

- [ ] **Phase 0 — Charter.** Manifesto, threat model, governance draft, ethics review.
- [ ] **Phase 1 — Resource Graph.** Open schema and public dataset aggregator.
- [ ] **Phase 2 — Simulator.** Sandboxed allocation models, evaluated on historical data.
- [ ] **Phase 3 — Ledger.** Reference implementation of the verifiable decision log.
- [ ] **Phase 4 — Pilots.** Voluntary, local, human-supervised deployments (e.g. a single supply chain).
- [ ] **Phase 5 — Federation.** Interoperation between independent nodes.

## Open problems

An honest project lists what it has not solved:

- **Legitimacy.** Who decides the objective function, and how is that choice made fairly?
- **Incentives.** Producers must keep a reason to produce; the protocol has to model this, not ignore it.
- **Data integrity.** Garbage or falsified inputs corrupt every downstream decision.
- **Adversaries.** A system this consequential is a target; security is a first-class design goal.
- **Safety.** Autonomy must be bounded; there must always be a reliable human override.
- **Medicine and IP.** Moving beyond patent barriers involves law, safety, quality control and incentives for research — not code alone.
- **Transition.** Real institutions, laws and people exist today; any path forward must work with them.

See [`MANIFESTO.md`](MANIFESTO.md) for the longer statement of intent.

## Contributing

We need economists, systems engineers, logisticians, cryptographers, ML researchers, public-health
experts, lawyers and critics. Open an issue with the label `RFC` to propose or challenge anything —
including the premise itself.

## License

AGPL-3.0 for code. CC BY-SA 4.0 for documentation and assets.
