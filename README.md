<p align="center">
  <img src="./Preview.png" width="500"/>
</p>

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


![Assembly Overview](images/overview.png)

### Motion Study
![Motion Study](motion-study.gif)

### Bill of Materials
![BOM](images/drawings/bom.png)



---
