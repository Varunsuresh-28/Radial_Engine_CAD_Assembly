# Radial Engine CAD Assembly 
**Tools:** SolidWorks | **Timeline:** December 2025 – February 2026

## Overview
5-cylinder radial engine modeled to understand the mechanical timing
of a main and articulated rod system.

## Key Work
- Circular Component Patterns and top-down design for scalability
- Motion Study to animate and verify kinematics, resolving interferences via FEA
- Structured BOM with traceable part references for assembly documentation

## Images

### Key Components Modeled
- **Main Rod**: primary connecting rod linking the crankshaft to the master piston
![Main Rod](./main-rod.png)

- **Articulated Rod**: secondary rods connecting the remaining 4 pistons to the main rod
![Articulated Rod](./Articulated-rod.png)

- **Piston**: top closure of each piston assembly, designed for precise fitment and clearance tolerances
![Piston](./piston.png)

- **Piston-Rod Subassembly**: isolated model of the piston joined to the main and articulated rods, showing the pin connections and joint geometry
![Piston-Rod Subassembly](./piston-rod-subassembly.png)

- **Crankshaft**: precision-machined rotating shaft converting reciprocating piston motion into continuous rotational output, with offset crank pins timed to coordinate the firing sequence across all 5 cylinders
![Crankshaft](./crankshaft.png)

- **Engine Shell (Crankcase & Cylinder Barrels)**: 5 cylinder central structural housing enclosing the crankshafts, Main Rod, Articulated Rods, and the Pistons. 
![Engine Shell](./engine-shell.png)

- **Propeller**: 3-blade propeller modeled using SolidWorks Sweep to generate the twisted aerofoil profile along a defined pitch path, simulating rotational output from the crankshaft
![Propeller](./propeller.png)

### Full Assembly
> Crankcase rendered transparent to expose the internal Piston-Rod Subassembly and crankshaft geometry

![Full Assembly](./full-assembly.png)

### Bill of Materials
> Full structured BOM with part numbers, descriptions, and quantities for all 12 components in the assembly.
<img src="./Radial-Engine-Bom.png" width="900"/>

### Motion Studies

- **Piston-Rod Subassembly Motion** — isolated animation of the piston, main rod, and articulated rod cycling through one full crankshaft revolution, validating pin joint kinematics and interference clearances

<img src="./piston-rod-motion.gif" width="1050"/>

- **Full Engine with Propeller** — complete 5-cylinder radial engine motion study with propeller attached, demonstrating synchronized firing sequence, rotational output, and propeller disc behavior under simulated load
<img src="./full-engine-propeller-motion.gif" width="1050"/>


## Finite Element Analysis (FEA) & Material Optimization

To validate the structural integrity of the engine block under simulated combustion loads and thermal stress, a progressive finite element analysis was conducted using SolidWorks Simulation. The study compared four distinct materials to determine the optimal balance of peak strength and minimum weight.

### Comparative Material Study

| Material | Yield Strength | Outcome |
|---|---|---|
| 1060-H12 Aluminum (Baseline) | ~75 MPa | Catastrophic failure — baseline only |
| 6061-T6 Aluminum | ~275 MPa | Significant deformation — failed peak stress requirements |
| 7075-T6 Aluminum | 505 MPa |  — optimal strength-to-weight ratio |
| AISI 4340 Steel (Normalized) | ~710 MPa | Structural fallback — excess weight penalty |

### Validation Results: 7075-T6 Aluminum

Testing the Engine Shell under steady-state thermal conditions (175°C – 230°C at cylinder heads) and peak mechanical combustion pressure.

| Parameter | Value |
|---|---|
| Maximum Stress (von Mises) | 361 MPa |
| Material Yield Strength | 505 MPa |
| Factor of Safety (FOS) | 1.4 |

### Engineering Conclusion

The 7075-T6 Aluminum alloy successfully withstands the simulated operating conditions without yielding. Because the peak stress (361 MPa) remains well below the material yield strength (505 MPa), the engine block operates entirely within its elastic region — flexing under load but returning to its original geometry without permanent deformation. The resulting Factor of Safety of 1.4 provides a 40% structural buffer, confirming the design achieves structural integrity while avoiding the weight penalty of a steel assembly.




---
