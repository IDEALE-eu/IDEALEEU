# Subsystem: 90-02_CBT_TRAINING_MODULES

## Description

Computer-Based Training (CBT) modules for IIF equipment operation and maintenance.

This subsystem contains interactive computer-based training modules, e-learning content, virtual simulations, and competency assessment tools for all IIF equipment and procedures.

## Parent System

[IIF-90_PROCEDURES_TRAINING](../../) - Procedures and Training system.

## PLM Structure

This subsystem contains engineering artifacts organized by CAx discipline:

### Engineering BOM
- [EBOM_LINKS.md](./PLM/EBOM_LINKS.md) - Links to authoritative ERP/PLM items

### CAx Directories

- [CAD/](./PLM/CAx/CAD/) - Computer-Aided Design (training interface designs, graphics)
- [CAE/](./PLM/CAx/CAE/) - Computer-Aided Engineering (training effectiveness analysis)
- [CAO/](./PLM/CAx/CAO/) - Computer-Aided Optimization (curriculum optimization)
- [CAM/](./PLM/CAx/CAM/) - Computer-Aided Manufacturing (content production workflows)
- [CAI/](./PLM/CAx/CAI/) - Computer-Aided Installation (LMS deployment procedures)
- [CAV/](./PLM/CAx/CAV/) - Computer-Aided Validation (training validation and assessment)
- [CAP/](./PLM/CAx/CAP/) - Computer-Aided Process Planning (training process design)
- [CAS/](./PLM/CAx/CAS/) - Computer-Aided Simulation (virtual training simulations)
- [CMP/](./PLM/CAx/CMP/) - Composite Materials Processing (multimedia content)

## Directory Structure

```
90-02_CBT_TRAINING_MODULES/
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
      ├─ CAP/
      ├─ CAS/
      └─ CMP/
```

## Working with This Subsystem

### Adding Engineering Artifacts
1. Place files in appropriate CAx subdirectory based on discipline
2. Use SCORM-compliant packages for LMS integration
3. Update `PLM/EBOM_LINKS.md` with ERP/PLM references
4. Follow naming conventions: `{MODULE_ID}_{DESCRIPTION}_{REV}.{ext}`

### BOM Management
Update [PLM/EBOM_LINKS.md](./PLM/EBOM_LINKS.md) with:
- Training module identifiers and versions
- Links to authoritative PLM/ERP systems
- Learning objectives and prerequisites
- Assessment criteria and passing scores

### File Formats
- **SCORM**: LMS-compatible training packages
- **HTML5**: Interactive web-based training
- **MP4**: Training videos
- **PDF**: Reference materials and job aids
- **JSON**: Assessment and quiz data

## Key Design Considerations

- SCORM 2004 compliance for LMS integration
- Accessibility standards (WCAG 2.1)
- Multi-language support
- Mobile device compatibility
- Offline capability for field training
- Progress tracking and competency assessment
- Interactive simulations and scenarios
- Gamification elements for engagement

## Navigation

- [⬆️ Back to IIF-90_PROCEDURES_TRAINING](../../)
- [📋 System Integration View](../../INTEGRATION_VIEW.md)
- [🔗 System Interfaces](../../INTERFACE_MATRIX/)
- [📂 All Subsystems](../)
- [🏠 SYSTEMS Home](../../../)

## References

- Parent System: [IIF-90_PROCEDURES_TRAINING](../../README.md)
- Interface Matrix: [../../INTERFACE_MATRIX/](../../INTERFACE_MATRIX/)
- Validation: `scripts/validate-structure.sh`

---

**Status**: Ready for engineering artifact population  
**Owner**: TBD - Assign subsystem engineer  
**Last Updated**: 2025-10-11
