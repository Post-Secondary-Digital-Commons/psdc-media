# Commons Media and Spatial Fabric

Media production and delivery ecosystem for image, video, 3D, and 4DGS assets.
It is a reusable Commons fabric deployed under each institution's data, rights,
privacy, and moderation authority.
It owns asset lifecycle, metadata, rights, moderation, generation pipelines,
transcoding, delivery, and spatial media workflows. Compute capacity is consumed
through Commons Compute Fabric/Commons Cloud Fabric contracts; social publishing is consumed through AC
Fediverse contracts.

## Ecosystem dependencies

Media Fabric depends on Commons Cloud Fabric for identity, policy, events, object-storage
interfaces, secrets, and observability. It requests compute from Commons Compute Fabric and AI
capabilities from Commons AI Fabric through versioned contracts. Publishing is delegated to
Commons Social Fabric; Media Fabric remains usable when federation is unavailable.

- [Consolidated ecosystem architecture](../psdc-architecture/docs/architecture/Consolidated-Ecosystem-Architecture.md)
- [Dependency contract](../psdc-architecture/docs/architecture/Ecosystem-Dependency-Contract.md)
- [Cross-pollination model](../psdc-architecture/docs/architecture/Cross-Pollination-and-Shared-Capabilities.md)
- [Open-source reference stack](../psdc-architecture/docs/vision/12-Open-Source-Reference-Stack.md)
- [Commons architecture](../psdc-architecture/docs/vision/constitutional/Post-Secondary-Digital-Commons-Architecture.md)

## Layout

- `apps/` — creator studio and administration clients
- `services/` — media API, registry, orchestration, metadata, delivery, moderation,
  and spatial services
- `pipelines/` — image, video, 3D, and 4DGS workflows
- `runtimes/` — pluggable generation and processing engines
- `connectors/` — cloud, compute, AI, and federated integrations
- `policies/` — safety, rights, and retention controls
