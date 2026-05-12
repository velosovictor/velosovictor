<div align="center">

# RationalBloks

### The industrial powerhouse of modular systems.

</div>

## Overview

RationalBloks is a deterministic verification infrastructure designed for highly coupled, safety-critical systems. Built to support **ISO 26262** workflows, it provides a mathematical framework to bypass the combinatorial explosions inherent in traditional Model-Based Systems Engineering (MBSE) state-machines.

While the industry relies heavily on explicit-state simulation to verify safety controllers and ADAS fusion platforms, RationalBloks utilizes a **Recursive Discrete Subtraction (RDS)** algorithm to geometrically isolate unmodeled states, specification voids, and rule conflicts directly from the control logic.

---

## Architecture & Workflow

### Step 1: Deterministic System Definition
Instead of relying on visual UIs, control logic and safety envelopes are defined via infrastructure-as-code. We utilize strict JSON schemas to guarantee Git-trackability, traceability, and mathematical rigor.

```json
{
  "safety_envelope": {
    "module": "start_stop_controller",
    "asil_target": "ASIL-D",
    "state_matrix": {
      "vehicle_speed": { "type": "float", "range": "[0, 250]" },
      "brake_pressure": { "type": "float", "range": "[0, 100]" },
      "gear_position": { "states": ["P", "R", "N", "D"] }
    },
    "transitions": [
      { "from": "engine_running", "to": "engine_standby", "condition": "speed == 0 && brake >= 50 && gear == D" }
    ]
  }
}
