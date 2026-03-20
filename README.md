# SwarmPlug Demo

## Foundation Layer Demonstration (ver0.1–ver0.4)

This repository contains the official demonstration media for the foundational infrastructure layers of SwarmPlug.

It presents observable system behavior only.  
No implementation artifacts are included.

---

## 🎥 Demo Coverage

### ver0.1–ver0.3
🎬 [Watch Demo Video](video/(ver0.1-ver0.3).mp4)

---

### ver0.4
🎬 Demo Videos:

- [Demo 01 — Testbed Overview](video/ver0.4/swarmplug-ver04-demo-01-testbed-overview.mp4)
- [Demo 02 — Single Producer → Single Receiver](video/ver0.4/swarmplug-ver04-demo-02-single-producer-single-receiver.mp4)
- [Demo 03 — Multi Producer → Single Receiver](video/ver0.4/swarmplug-ver04-demo-03-multi-producer-single-receiver.mp4)
- [Demo 04 — Single Producer → Multi Receiver](video/ver0.4/swarmplug-ver04-demo-04-single-producer-multi-receiver.mp4)
- [Demo 05 — Full Mesh Stability](video/ver0.4/swarmplug-ver04-demo-05-full-mesh-stability.mp4)

---

## Demonstrated Capabilities

The demonstration media in this repository cover the first four infrastructure layers of SwarmPlug.

### ver0.1 — Host Attachment
- Deterministic connection to ROS runtime  
- Discovery of topics, services, and parameters  

### ver0.2 — Canonical Identity
- Stable host identity anchor  
- Canonical node identification across heterogeneous hosts  

### ver0.3 — Semantic Snapshot
- Deterministic semantic snapshot generation  
- Structured state exposure at the infrastructure boundary  
- Event-based and periodic trigger behavior  

### ver0.4 — Mesh Snapshot Exchange
- Cross-node semantic snapshot delivery over the mesh layer  
- Single-producer and multi-producer transmission patterns  
- Single-receiver and multi-receiver dissemination behavior  
- Concurrent multi-node exchange under full-mesh conditions  
- Stable communication behavior without recursive re-forwarding  
- No message storm caused by received-message rebroadcast loops  

---

## Video Index

### ver0.1–ver0.3
- **Foundation Demo Video**  
  Demonstrates the progression from host attachment to semantic snapshot generation.  

### ver0.4

- **Demo 01 — Testbed Overview**  
  Overview of the SwarmPlug ver0.4 multi-node testbed.  

- **Demo 02 — Single Producer → Single Receiver**  
  Point-to-point semantic snapshot delivery.  

- **Demo 03 — Multi Producer → Single Receiver**  
  Multi-source concurrent snapshot delivery.  

- **Demo 04 — Single Producer → Multi Receiver**  
  One-to-many dissemination over mesh.  

- **Demo 05 — Full Mesh Stability**  
  Full-mesh exchange stability without message storm.  

---

## Scope

This repository demonstrates:

- Observable system behavior  
- Version-scoped capabilities  
- Layered infrastructure progression  
- Multi-node communication behavior in ver0.4  
- Public-facing demonstration milestones only  

It does **not** include:

- Source code  
- Configuration files  
- Internal schemas  
- Core algorithms  
- Deployment instructions  
- Reproducible implementation details  

This repository is not a setup guide and is not intended for reproduction.

---

## Version Policy

Each version is demonstrated as an independent, version-scoped milestone.

The current demo coverage includes:

- ver0.1 — Host Attachment  
- ver0.2 — Canonical Identity  
- ver0.3 — Semantic Snapshot  
- ver0.4 — Mesh Snapshot Exchange  

Future versions will be added only when clearly defined and externally demonstrable.

---

## Repository Positioning

This repository serves as a public-facing demonstration archive for SwarmPlug milestone behavior.

Its purpose is to document visible infrastructure outcomes at each version boundary, while keeping implementation logic and core system mechanisms outside the scope of public release.

---

## License

This repository is licensed under the **SwarmPlug Demo Media License v1.0**.

See the `LICENSE` file for details.

---

## Contact

📧 swarmplug@gmail.com
