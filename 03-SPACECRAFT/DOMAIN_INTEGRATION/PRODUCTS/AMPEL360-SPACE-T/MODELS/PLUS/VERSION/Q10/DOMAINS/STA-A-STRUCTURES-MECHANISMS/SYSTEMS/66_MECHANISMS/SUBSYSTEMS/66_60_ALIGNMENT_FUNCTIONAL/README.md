# Subsystem: 66_60_ALIGNMENT_FUNCTIONAL

## Description

Alignment verification and functional positioning.

## Parent System

[66_MECHANISMS](../../) - Release devices, hinges, bearings, deployable mechanisms, and associated actuation systems.

## PLM Structure

This subsystem contains engineering artifacts organized by CAx discipline:

### Engineering BOM
- [EBOM_LINKS.md](./PLM/EBOM_LINKS.md) - Links to authoritative ERP/PLM items

### CAx Directories

- [CAD/](./PLM/CAx/CAD/) - Computer-Aided Design (3D models, drawings)
- [CAE/](./PLM/CAx/CAE/) - Computer-Aided Engineering (FEA, analysis)
- [CAO/](./PLM/CAx/CAO/) - Computer-Aided Optimization (design optimization)
- [CAM/](./PLM/CAx/CAM/) - Computer-Aided Manufacturing (NC programming, tooling)
- [CAI/](./PLM/CAx/CAI/) - Computer-Aided Installation (installation drawings, procedures)
- [CAV/](./PLM/CAx/CAV/) - Computer-Aided Validation (test models, validation data)
- [CAS/](./PLM/CAx/CAS/) - Computer-Aided Simulation (system simulations)
- [CMP/](./PLM/CAx/CMP/) - Composite Materials Processing (layup data, curing)

## Directory Structure

```
66_60_ALIGNMENT_FUNCTIONAL/
├─ README.md (this file)
└─ PLM/
   ├─ EBOM_LINKS.md
   └─ CAx/
      ├─ CAD/
      ├─ CAE/
      ├─ CAO/
      ├─ CAM/
      ├─ CAI/
      ├─ CAV/
      ├─ CAS/
      └─ CMP/
```

## Working with This Subsystem

### Adding Engineering Artifacts
1. Place files in appropriate CAx subdirectory based on discipline
2. Use neutral formats (STEP, JT, glTF) alongside native where possible
3. Update `PLM/EBOM_LINKS.md` with ERP/PLM references
4. Follow naming conventions: `{PART_ID}_{DESCRIPTION}_{REV}.{ext}`

### BOM Management
Update [PLM/EBOM_LINKS.md](./PLM/EBOM_LINKS.md) with:
- Part numbers and sourcing information
- Links to authoritative PLM/ERP systems
- Configuration control references
- Supplier information

### File Formats
- **CAD**: STEP, JT, native CAD formats
- **CAE**: Nastran, ANSYS, solver input/output
- **CAM**: CNC programs, tooling definitions
- **Documents**: PDF for controlled documents

## Navigation

- [⬆️ Back to 66_MECHANISMS](../../)
- [📋 System Integration View](../../INTEGRATION_VIEW.md)
- [🔗 System Interfaces](../../INTERFACE_MATRIX/)
- [📂 All Subsystems](../)
- [🏠 SYSTEMS Home](../../../)

## References

- Parent System: [66_MECHANISMS](../../README.md)
- Interface Matrix: [../../INTERFACE_MATRIX/](../../INTERFACE_MATRIX/)
- Validation: `scripts/validate-spacecraft-systems.sh`

---

**Status**: Ready for engineering artifact population  
**Owner**: TBD - Assign subsystem engineer  
**Last Updated**: 2025-10-10
