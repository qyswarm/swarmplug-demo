# Demo Scenario – SwarmPlug v0.2

This document describes the **experimental scenario** used in the SwarmPlug v0.2 demo video.

It is intended to clarify **what environment the demo was recorded in**,  
and **what the demo does and does not claim to demonstrate**.

No implementation details are disclosed here.

---

## 1. Demo Objective

The purpose of this demo is to demonstrate **SwarmPlug v0.2 as a structural clarity layer for ROS systems**, specifically:

- Canonical naming of ROS resources
    
- Explicit host identity attribution
    
- Read-only introspection of an existing ROS system
    

This demo does **not** demonstrate control, coordination, or communication mechanisms.

---

## 2. System Roles

### 2.1 ROS Host (Unmodified)

The ROS host is a **standard ROS1 system**, running typical application nodes.

- **ROS version:** ROS1 Noetic
    
- **Role:**
    
    - Runs `roscore`
        
    - Runs application nodes
        
    - Provides the ROS graph
        

The ROS host:

- Does **not** install SwarmPlug
    
- Does **not** run any SwarmPlug-related code
    
- Is completely unaware of SwarmPlug’s existence
    

This ensures that SwarmPlug operates as a **non-intrusive sidecar module**.

---

### 2.2 SwarmPlug Plugin Device

SwarmPlug runs on a **separate device** and attaches to the ROS host externally.

- **SwarmPlug version:** v0.2
    
- **Mode:** CLI-based, read-only inspection
    
- **Responsibilities:**
    
    - Discover and bind to the ROS host
        
    - Export ROS environment variables locally
        
    - Provide structured CLI outputs
        

The plugin device does **not** start any ROS application nodes.

---

## 3. Application Stack on the ROS Host

The ROS host runs two representative workloads:

### 3.1 `turtlesim`

- Simple, well-known ROS demo application
    
- Provides:
    
    - Topics
        
    - Services
        
    - Parameters
        

`turtlesim` is used to demonstrate **clarity and accessibility**.

---

### 3.2 `mavros`

- A complex, production-grade ROS integration layer
    
- Provides:
    
    - A large number of topics and services
        
    - Deep namespace hierarchies
        

`mavros` is used to demonstrate **scalability and structural consistency** under complexity.

---

## 4. Demonstrated Capabilities

The demo video shows the following SwarmPlug v0.2 capabilities:

- Automatic attachment to an existing ROS master
    
- Canonical naming for:
    
    - Topics
        
    - Services
        
    - Parameters
        
    - Actions (topology inference)
        
- Explicit host identity resolution
    
- Host network self-description (preferred IP/MAC)
    

All operations are **read-only**.

---

## 5. Canonical Naming Scope

Canonical names follow the format:

```
/sp/<host_id>/<kind>/<ros_path>
```

Where:

- `<host_id>` identifies the plugin host
    
- `<kind>` is one of: `topic`, `service`, `param`, `node`, `action`
    
- `<ros_path>` is the original ROS name
    

Canonical names:

- Do **not** replace ROS names
    
- Do **not** alter the ROS graph
    
- Are used purely as **structural references**
    

---

## 6. What Is Explicitly Not Demonstrated

To avoid ambiguity, this demo intentionally does **not** include:

- Robot or vehicle control
    
- Parameter modification
    
- Service invocation
    
- Cross-host communication
    
- Multi-master setups
    
- Mesh, blockchain, or consensus mechanisms
    

These features are **out of scope** for SwarmPlug v0.2.

---

## 7. Interpretation Guidance

This demo should be interpreted as:

> A demonstration of **system observability, attribution, and structural clarity**  
> for existing ROS deployments.

It is **not** a complete system solution, nor a coordination framework.

---

## 8. Version Context

- **Version:** SwarmPlug v0.2
    
- **Status:** Engineering Stable
    
- **Position in roadmap:**
    
    - v0.1 – Host discovery & safe binding
        
    - v0.2 – Canonical naming & host identity (**this demo**)
        
    - v0.3 – Unified parameter/state schema (planned)
