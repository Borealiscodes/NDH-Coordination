# ⭐ **NDH‑Coordination Provenance Passive Interface v1.0**  
### *Passive Boundary • Lineage Routing • Altitude‑Neutral Interface*

## **1. Purpose**

This passive interface defines **how NDH‑Coordination interacts with the Provenance Layer**, the subsystem responsible for:

- lineage  
- anchors  
- origin metadata  
- artifact history  
- versioning  
- architectural ancestry  

Coordination does **not**:

- rewrite provenance  
- generate provenance  
- interpret provenance  
- validate provenance  
- enforce provenance rules  

It only **routes provenance metadata** upward.

---

## ⭐ **2. Interface Role**

The Provenance Layer is the **lineage altitude** of NDH.

Coordination’s role is to:

- detect missing provenance  
- isolate provenance metadata  
- preserve anchor structure  
- route provenance upward  
- prevent provenance omission drift  
- maintain NDH’s historical coherence  

This interface defines that boundary.

---

## ⭐ **3. Provenance Indicators (Passive)**

Coordination identifies provenance using **passive indicators**, not interpretation:

- presence of a provenance footer  
- presence of anchors  
- presence of version metadata  
- presence of maintainer metadata  
- presence of location metadata  
- presence of artifact lineage  
- absence of any of the above (omission drift)

These indicators trigger routing to the Provenance Layer.

---

## ⭐ **4. Passive Interface Table (v1.0)**

| Component Type | Indicator | Routing Behavior | Notes |
|----------------|-----------|------------------|-------|
| **Provenance Footer** | presence of footer block | Route to **Provenance Layer** | Preserve exactly |
| **Anchor List** | list of referenced artifacts | Route to Provenance | No validation |
| **Version Metadata** | version numbers, draft markers | Route to Provenance | Non‑interpretive |
| **Maintainer Metadata** | author, location, timestamp | Route to Provenance | Non‑evaluative |
| **Lineage Metadata** | origin, ancestry, architectural history | Route to Provenance | Non‑activating |
| **Omission Drift** | missing provenance footer | Route to Provenance | Add drift log only |

This table defines the **provenance boundary**.

---

## ⭐ **5. Interface Rules**

### **Rule 1 — Passive Only**  
Coordination does not interpret provenance meaning.

### **Rule 2 — Non‑Destructive**  
Provenance metadata is preserved exactly as written.

### **Rule 3 — No Provenance Generation**  
Coordination does not create provenance; it only routes it.

### **Rule 4 — No Provenance Validation**  
Coordination does not check correctness or completeness.

### **Rule 5 — Omission Drift Logging**  
Missing provenance triggers a drift log, not a rewrite.

---

## ⭐ **6. Routing Flow**

```
Artifact enters Coordination
   ↓ detect provenance indicators
Isolate provenance metadata
   ↓ route to Provenance Layer
Preserve anchor structure
   ↓ prevent provenance omission drift
Coordination remains altitude-neutral
```

This is the correct provenance routing posture.

---

## ⭐ **7. Provenance Footer — Provenance Passive Interface v1.0**

```
---
Artifact: NDH-Coordination Provenance Passive Interface v1.0
Lane: NDH-COORDINATION • Passive Interface • Draft

Purpose:
Define passive lineage boundary between NDH-Coordination and the Provenance
Layer. Enables altitude-neutral routing of provenance metadata without
interpretation, validation, or rewriting.

Anchors:
  NDH-Coordination Roadmap v1.0
  NDH-Coordination-AltitudeMap_v1_0
  NDH-Coordination-SubsystemMap_v1_0
  NDH-Coordination-DriftIndicatorsSpec_v1_0
  NDH-Coordination-AltitudeSeparationSpec_v1_0

Maintainer: Borealis S. Hedling
Location: Dublin, Ireland • 2026
Version: v1.0
---
```

---

