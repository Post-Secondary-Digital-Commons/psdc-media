# Commons Media and Spatial Fabric Overview

```text
client -> media API -> asset registry -> job orchestrator
                                      -> approved runtime or Commons Compute Fabric job
                                      -> metadata/provenance
                                      -> delivery
```

Assets, manifests, jobs, outputs, and renditions have separate identities. Every
generated or transformed asset records its inputs, pipeline version, runtime,
policy result, and spatial metadata when applicable.
