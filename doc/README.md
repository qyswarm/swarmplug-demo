### SwarmPlug Demo Repository

This repository contains **demonstration materials only** for SwarmPlug.

It does **not** include source code, implementation details, or internal logic.

---

### 🎥 SwarmPlug v0.2 – Canonical Naming Demo

📌 **Version:** v0.2  
📌 **Focus:** Canonical Naming & Host Identity  
📌 **Scope:** Read-only, non-intrusive ROS introspection

👉 **Watch the demo video:**  
`videos/swarmplug_v0.2_demo.mp4`

---

### What This Demo Shows

- Attaching SwarmPlug to an **existing ROS1 host**
    
- No modification to the host system
    
- Canonical naming for:
    
    - topics
        
    - services
        
    - parameters
        
    - actions
        
- Explicit host identity and network self-description
    

---

### What This Demo Does NOT Show

- No robot control
    
- No parameter modification
    
- No cross-host communication
    
- No mesh, blockchain, or consensus logic
    

This demo is strictly **structural and observational**.

---

### Demo Scenario

- **ROS Host:**
    
    - ROS1 Noetic
        
    - `turtlesim`
        
    - `mavros`
        
- **Plugin Device:**
    
    - SwarmPlug v0.2
        
    - CLI-based inspection only
        

The ROS host is **unmodified** and **does not run SwarmPlug**.

---

### Project Context

This demo corresponds to **SwarmPlug v0.2**, which introduces:

- Canonical naming layer
    
- Explicit host identity abstraction
    
- Network self-description for plugin devices
    

For architectural context, see the main repository:  
👉 `swarmplug` (documentation-only)

---

### License & Notice

This repository is for **demonstration and evaluation purposes only**.

No permission is granted to infer or reimplement internal mechanisms based on this material.
