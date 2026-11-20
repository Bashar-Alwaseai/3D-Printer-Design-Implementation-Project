#  3D Printer Design & Implementation Project

Collaborated with an engineering team to design and build a functional FDM 3D printer. The project involved CAD-based mechanical design, integration of stepper motors and linear motion systems, microcontroller control, and motion programming to achieve accurate and reliable 3D printing performance.

---

##  Mechanical Design
The complete mechanical design was developed in **SolidWorks**, covering every component of the printer from the structural frame to the motion systems. The design is fully parametric and organized as assembly-ready models, so each part can be inspected, modified, manufactured, and assembled.

**Design deliverables**
- **Individual parts:** all printer components modeled as separate SolidWorks part files (`.SLDPRT`).
- **Sub-assemblies:** frame, X/Y/Z motion axes, extruder carriage, and heated bed assemblies (`.SLDASM`).
- **Full printer assembly:** the complete machine with mates and constraints, ready for assembly verification and motion checks.
- **Neutral formats:** STEP and STL files for use in other CAD software or for direct 3D printing of parts.

**Engineering analysis**
- Structural stress analysis was performed on critical components (such as the lead screw and key structural parts) to verify strength and reliability under working loads. Result images are available in the `Images for stress analysis` folder.

---

## 📥 Download the CAD Files
All SolidWorks parts, assemblies, and exported formats are available in the **Releases** tab:

👉 **[Download the design files from Releases](https://github.com/Bashar-Alwaseai/3D-Printer-Design-Implementation-Project/releases)**

The package includes:

| File type | Description |
|---|---|
| `.SLDPRT` | Individual part models |
| `.SLDASM` | Sub-assemblies and the full printer assembly |
| `.STEP` | Universal CAD format for use in any CAD software |
| `.STL` | Ready-to-print part files |

>  Keep all files in the same folder after extracting so SolidWorks assemblies can find their referenced parts.

---

##  Motion System & Electronics

- **Motion:** stepper motors driving linear motion axes through lead screws and linear guides, including an 8 mm × 500 mm lead screw for the vertical axis.
- **Controller:** microcontroller-based control board running the printer firmware.
- **Firmware:** **Marlin 2.1.2.5**, configured for the printer's kinematics, motor settings, and endstops.
- **Heating:** [hotend and heated bed details].

---

##  Firmware & Motion Programming

The `Code` folder contains the firmware source and configuration used to control the printer, including:

- Marlin 2.1.2.5 firmware with the printer-specific configuration
- Motion parameters such as steps per mm, maximum speeds, and acceleration
- Endstop and homing configuration

---

##  Repository Structure

```
├── Code/                        # Firmware (Marlin 2.1.2.5) and configuration
├── Images for stress analysis/  # Stress analysis results
├── The program used/            # Software used (Printrun, Slic3r)
├── Video/                       # Project demonstration videos
└── README.md
```

---

##  Software Used

- **SolidWorks:** mechanical design, assemblies, and stress analysis
- **Marlin 2.1.2.5:** printer firmware
- **Printrun / Slic3r:** printer control and slicing

---

## Specifications

| Specification | Value |
|---|---|
| Printing technology | FDM (Fused Deposition Modeling) |
| Build volume | X × Y × Z mm |
| Filament diameter | 1.75 mm |
| Nozzle diameter | 0.4 mm |
| Controller board | Arduino Mega |
| Firmware | Marlin 2.1.2.5 |

...
