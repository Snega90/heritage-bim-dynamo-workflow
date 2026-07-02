# Heritage & BIM Dynamo Automation Scripts

> Open-source Dynamo graphs automating ISO 19650-compliant documentation and Room/Space management workflows in Autodesk Revit, developed through independent professional practice and MSc research into AI-augmented heritage BIM retrofit.

## Overview

This repository contains two Dynamo automation tools developed to reduce manual, repetitive tasks in BIM documentation and heritage retrofit modelling:

1. **ISO 19650 Sheet Naming Automation** — automatically generates and applies ISO 19650-compliant sheet naming conventions across a Revit project.
2. **Room/Space Selection & Management** — automates the selection, listing, and cleanup of Rooms and Spaces ahead of energy simulation handoff (e.g. to IESVE via Pollination).

Both scripts were developed and tested in live professional and research contexts and are shared here so other BIM practitioners, students, and researchers can adapt them for their own projects.

## What's in this repo

| File | Description |
|---|---|
| `iso19650-sheet-naming.dyn` | Automatically names/renames Revit sheets per ISO 19650 naming convention |
| `clear-rooms-and-spaces.dyn` | Clears/deletes existing Spaces ahead of regeneration |
| `LICENSE` | MIT License |

## Requirements

- Autodesk Revit *(add your version, e.g. 2024/2025)*
- Dynamo *(add version bundled with your Revit, e.g. 2.x)*
- Required packages: *(list any non-default packages here — e.g. Clockwork, archi-lab, Rhythm — with version numbers; leave blank if none used)*

## How to use

### ISO 19650 Sheet Naming
1. Open the project in Revit and launch Dynamo.
2. Open `scripts/iso19650-sheet-naming.dyn`.
3. Update the project/originator/zone/level codes in the input nodes to match your own ISO 19650 container naming structure.
4. Run — sheet names/titles update automatically across the selected sheet set.

### Room/Space Management
1. Open `scripts/select-spaces-rooms.dyn` (or `clear-spaces.dyn` to reset existing Spaces first).
2. Confirm the category filters match your model's Room/Space setup.
3. Run to batch-select, list, or clear Rooms/Spaces ahead of further processing (e.g. export for energy simulation).

## Background

The ISO 19650 sheet naming script was originally developed for professional project documentation use and shared on LinkedIn, where it received positive feedback from the BIM community. The Room/Space scripts were developed as part of MSc research into AI-augmented HBIM workflows for heritage retrofit, supporting the transfer of Revit models into environmental simulation software.

## Licensing

This repository is released under the [MIT License](./LICENSE) — free to use, modify, and redistribute, including commercially, provided the original copyright notice is retained.

## Citation

If you use or build on this work, please cite:

> Raja Sekar, S. (2025). *Heritage & BIM Dynamo Automation Scripts* [Software]. GitHub.
> Zenodo archive: https://doi.org/10.5281/zenodo.21137964

## Author

**Snega Raja Sekar** — Architect (India) | Architectural Technologist (UK) | BIM Technician

## Disclaimer

This repository does not include any client-specific project data, drawings, or identifying site information. Scripts are generalised for reuse across BIM projects.
