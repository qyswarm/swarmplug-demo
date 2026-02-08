# SwarmPlug Demo

**Demonstration Repository for SwarmPlug (Public, Read-Only)**

This repository contains **demonstration materials only** for the SwarmPlug project.  
It is intended to provide **observable evidence of system behavior**, not source code or implementation details.

> This repository complements the main `swarmplug` repository,  
> which defines the overall architecture and version roadmap.

---

## What This Repository Is

This repository serves as a **demo and evaluation hub** for SwarmPlug.

It provides:

- Recorded demo videos  
- Demo scenario descriptions  
- Observable CLI outputs and system behavior  
- Public, verifiable release timestamps  

The goal is to show **what SwarmPlug does**, not **how it is implemented**.

---

## What This Repository Is NOT

To avoid ambiguity, this repository does **not** include:

- SwarmPlug source code  
- Core synchronization or coordination logic  
- Internal protocols or optimizations  
- Appliance images or firmware  
- Configuration scripts or deployment instructions  

All internal implementations remain **private by design**.

---

## Current Demo: SwarmPlug v0.2

### Demo Focus

The current demo corresponds to **SwarmPlug v0.2**, which introduces:

- Canonical naming of ROS resources  
- Explicit host identity abstraction  
- Read-only introspection of existing ROS systems  
- Host network self-description (preferred IP / MAC)  

This demo is **structural and observational**.

---

### What the Demo Shows

- Attaching SwarmPlug to an **unmodified ROS1 host**  
- No installation or configuration on the ROS host  
- Canonical naming for:
  - topics  
  - services  
  - parameters  
  - actions  
- Unified CLI-based system inspection  

---

### What the Demo Does NOT Show

- No robot or vehicle control  
- No parameter modification  
- No service invocation  
- No cross-host synchronization  
- No mesh, blockchain, or consensus logic  

This is intentional and consistent with the scope of v0.2.

---

## Demo Scenario Overview

The demo video is recorded in a minimal but representative setup:

- **ROS Host**
  - ROS1 (Noetic)
  - Runs standard applications (e.g. `turtlesim`, `mavros`)
  - Completely unmodified

- **SwarmPlug Plugin Device**
  - Runs SwarmPlug v0.2
  - Attaches as a sidecar
  - Uses CLI-based, read-only inspection

A detailed description is available in:

docs/demo_scenario.md


---

## Demo Video

**SwarmPlug v0.2 – Canonical Naming & Host Identity Demo**

The demo video shows real terminal output and system behavior.  
It is intended for:

- ROS system engineers  
- Robotics infrastructure researchers  
- Architecture-oriented reviewers  

See the `videos/` directory for the full recording.

---

## Relationship to the Main Repository

- **swarmplug**
  - Architecture, philosophy, and version roadmap
  - Documentation-focused

- **swarmplug-demo** (this repository)
  - Behavioral evidence and recorded demos
  - No implementation details

Together, these repositories provide a **clear separation between design intent and observable behavior**.

---

## Versioning & Updates

- Current demo version: **v0.2**
- This README will be updated as new demo versions are added
- Older demos may remain available for historical reference

---

## License & Notice

This repository is provided **for demonstration and evaluation purposes only**.

No permission is granted to infer, re-implement, or reverse-engineer internal mechanisms based on these materials.

---

## Contact

For collaboration, evaluation, or commercial inquiries:

- swarmplug@163.com  
- swarmplug@gmail.com
