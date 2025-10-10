# System 84: ELECTRIC_PROPULSION

## System Overview

**Description:** Electric propulsion systems including thrusters and Power Processing Unit (PPU) interfaces. If applicable to mission.

**System ID:** 84  
**Total Subsystems:** 2  
**Interface Matrix:** [84↔21_24_28_72_97.csv](./INTERFACE_MATRIX/84↔21_24_28_72_97.csv)

## Purpose

This system provides integration and coordination for all ELECTRIC_PROPULSION subsystems within the AMPEL360-SPACE-T spacecraft. It serves as:

- **Integration Anchor**: Central coordination point for subsystem interfaces
- **Interface Definition**: Manages system-to-system interface requirements
- **Configuration Control**: Ensures subsystem compatibility and integration

**Note:** This system is only applicable if the mission includes electric propulsion capabilities.

## Quick Navigation

- [📋 System README](./README.md) - Detailed system documentation
- [🔗 Interface Matrix](./INTERFACE_MATRIX/) - System interface definitions
- [📂 Subsystems](./SUBSYSTEMS/) - Access all subsystems
- [🏠 SYSTEMS Home](../README.md) - Return to main SYSTEMS directory

## Subsystems

| ID | Subsystem | Description |
|----|-----------|-------------|
| 10 | [84-10_THRUSTERS](./SUBSYSTEMS/84-10_THRUSTERS/) | Electric propulsion thrusters (ion, Hall effect, etc.). |
| 20 | [84-20_PPU_INTERFACES](./SUBSYSTEMS/84-20_PPU_INTERFACES/) | Power Processing Unit (PPU) interfaces and power management. |

## System Interfaces

The [Interface Matrix](./INTERFACE_MATRIX/) directory contains CSV files defining interfaces with other systems:

- Interface requirements and specifications
- Physical interfaces (mechanical, electrical, fluid)
- Functional interfaces (data, commands)
- Verification and validation approach

### Key Interfacing Systems

- **21-THERMAL_CONTROL**: Thermal management for EP thrusters
- **24-ELECTRICAL_POWER_EPS**: High-power interfaces to PPU
- **28-PROPELLANT_SYSTEMS**: Propellant (xenon, krypton, etc.) feed
- **72-PROPULSION_THRUST_DEVICES**: Propulsion coordination
- **97-ELECTRICAL_HARNESS**: Electrical connections

### Interface Management Process

1. **Define**: Document interface requirements in CSV format
2. **Review**: Coordinate with interfacing system teams
3. **Implement**: Develop interface control documents (ICDs)
4. **Verify**: Validate interfaces during integration testing

## Integration Workflow

### For System Engineers

1. **Planning Phase**
   - Review subsystem requirements
   - Define system-level interfaces
   - Develop integration sequence

2. **Implementation Phase**
   - Coordinate subsystem development
   - Manage interface definitions
   - Track integration readiness

3. **Verification Phase**
   - Verify system-level requirements
   - Validate interface compliance
   - Conduct integration testing

### For Subsystem Engineers

1. **Access Your Subsystem**
   - Navigate to `SUBSYSTEMS/{YOUR_SUBSYSTEM}/`
   - Review subsystem README for requirements

2. **Develop Artifacts**
   - Place engineering files in `PLM/CAx/` subdirectories
   - Update `PLM/EBOM_LINKS.md` for BOM references

3. **Interface Coordination**
   - Review interface matrix for your subsystem
   - Coordinate with interfacing subsystems
   - Update ICDs as needed

## Documentation Structure

```
{SYSTEM}/
├─ README.md                    # Detailed system documentation
├─ INTEGRATION_VIEW.md          # This file - integration overview
├─ INTERFACE_MATRIX/            # System interface definitions
│  └─ *.csv                     # Interface requirement CSVs
└─ SUBSYSTEMS/                  # All subsystems for this system
   └─ {SUBSYSTEM}/
      ├─ README.md              # Subsystem documentation
      └─ PLM/                   # Engineering artifacts
         ├─ EBOM_LINKS.md       # BOM references
         └─ CAx/                # CAx artifacts by discipline
            ├─ CAD/
            ├─ CAE/
            ├─ CAO/
            ├─ CAM/
            ├─ CAI/
            ├─ CAV/
            ├─ CAS/
            └─ CMP/
```

## Configuration Management

### Change Control

- All interface changes require CCB approval
- Update interface matrix CSV files for changes
- Coordinate with affected subsystems
- Update ICDs and trace to requirements

### Baseline Management

- System baselines established per program milestones
- Subsystem PLM artifacts tracked in ERP/PLM system
- Interface definitions under configuration control

## References

- [Main SYSTEMS README](../README.md)
- Configuration Management: `00-PROGRAM/CONFIG_MGMT/`
- Validation: `scripts/validate-spacecraft-systems.sh`
- Interface Requirements: See `INTERFACE_MATRIX/*.csv`

---

**Status**: Structure ready for subsystem population  
**Integration Lead**: TBD  
**Last Updated**: 2025-10-10
