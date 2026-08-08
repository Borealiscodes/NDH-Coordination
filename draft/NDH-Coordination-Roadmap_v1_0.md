# ⭐ **NDH‑Coordination Roadmap v1.0**  
### *Repo‑Scaffold Alignment • Build Sequence • Dependency Geometry*

## **1. Purpose of This Roadmap**

The README for NDH‑Coordination is intentionally **fully scaffolded**, listing:

- JSON routing maps  
- passive interfaces  
- stability specs  
- drift‑prevention rules  
- test harnesses  

But the repo currently contains only:

- Routing Table v1.0  
- Altitude Map v1.0  
- Coordination Layer Draft  
- Case Study v0.9  

This roadmap defines **how to build the rest**, in the correct altitude order, without drift or subsystem contamination.

---

## ⭐ **2. Roadmap Overview (v1.0)**

NDH‑Coordination must be built in **three phases**:

### **Phase 1 — Structural Geometry (You are here)**  
Artifacts that define the *shape* of Coordination:

- **Routing Table**  
- **Altitude Map**  
- **Subsystem Map**  

These establish the altitude membrane.

### **Phase 2 — Stability Layer**  
Artifacts that prevent drift:

- **Drift Indicators Spec**  
- **Altitude Separation Spec**  
- **stability/drift_prevention.md**  
- **stability/altitude_separation.md**

These ensure Coordination remains neutral.

### **Phase 3 — Passive Interfaces + Tests**  
Artifacts that connect Coordination to other NDH subsystems:

- **interfaces/constellation.passive.md**  
- **interfaces/provenance.passive.md**  
- **interfaces/triadic_core.passive.md**  
- **interfaces/simulation_suite.passive.md**  
- **interfaces/research_pilot.passive.md**

And the test harness:

- **tests/routing_sanity_test.md**  
- **tests/drift_prevention_test.md**  
- **tests/altitude_boundary_test.md**

These ensure Coordination routes correctly without activating anything.

---

## ⭐ **3. Roadmap Table (v1.0)**

| Stage | Artifact | Status | Dependency |  
|-------|----------|--------|------------|  
| **1.1** | **Routing Table v1.0** | ✔️ Complete | None |  
| **1.2** | **Altitude Map v1.0** | ✔️ Complete | Routing Table |  
| **1.3** | **Subsystem Map v1.0** | ⏳ Pending | Altitude Map |  
| **2.1** | **Drift Indicators Spec** | ⏳ Pending | Subsystem Map |  
| **2.2** | **Altitude Separation Spec** | ⏳ Pending | Drift Indicators |  
| **3.1** | constellation.passive.md | ⏳ Pending | Separation Spec |  
| **3.2** | provenance.passive.md | ⏳ Pending | Separation Spec |  
| **3.3** | triadic_core.passive.md | ⏳ Pending | Separation Spec |  
| **3.4** | simulation_suite.passive.md | ⏳ Pending | Separation Spec |  
| **3.5** | research_pilot.passive.md | ⏳ Pending | Separation Spec |  
| **3.6** | routing_sanity_test.md | ⏳ Pending | All passive interfaces |  
| **3.7** | drift_prevention_test.md | ⏳ Pending | Stability Layer |  
| **3.8** | altitude_boundary_test.md | ⏳ Pending | Stability Layer |

This table is the authoritative build sequence.

---

## ⭐ **4. README Alignment Notes**

The README currently lists:

```
src/routing/
src/interfaces/
src/stability/
tests/
```

This roadmap ensures:

- every folder will be populated  
- every JSON will be created  
- every passive interface will exist  
- every stability rule will be implemented  
- every test will be written  

Once Phase 1–3 are complete, the README will be **fully aligned** with the repo.

---

## ⭐ **5. Provenance Footer — Coordination Roadmap v1.0**

```
---
Artifact: NDH-Coordination Roadmap v1.0
Lane: NDH-COORDINATION • Repo Root • Planning

Purpose:
Define the build sequence, dependencies, and structural geometry required to
complete NDH-Coordination as a routing-only, altitude-neutral subsystem. Ensures
alignment between README scaffold and actual artifacts.

Anchors:
  NDH-Coordination README v2.0
  Coordination-Routing-Table_v1_0
  NDH-Coordination-AltitudeMap_v1_0

Maintainer: Borealis S. Hedling
Location: Dublin, Ireland • 2026
Version: v1.0
---
```

---

