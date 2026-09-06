# AutomationML libraries for graphical description languages

CAEX class libraries that represent two graphical description languages in AutomationML, plus an example where models of both languages sit in one document next to a plant hierarchy.

## Files

- `VDI_FPD_DomainLibrary_v0.7.aml` – Formalized Process Description (VDI/VDE 3682). Decomposition and boundary states use the reference attribute types of the AutomationML ObjectReferences library.
- `ISO_PT_DomainLibrary_v0.2.aml` – basic place/transition Petri nets (ISO/IEC 15909-1). Arcs are InternalElements with their own interfaces.
- `OMG_DD_AttributeTypeLib_v0.1.aml` – diagram-interchange attribute types (bounds, point, waypoint) after the OMG Diagram Definition. Used by both domain libraries.
- `BridgingExample_MPS500.aml` – Festo MPS500: FPD process view, Petri net of the quality-check station, and plant hierarchy in one file. Resources and Petri net nodes are linked to the plant with InternalLinks, the MPS500 resource with `refBaseObj`.
- `MPS500.json` – the FPD process model of the MPS500 from the FPB.JS editor.

## Opening the files

The AML files reference each other by file name, so keep them in one folder.

Not included, add them in the AML Editor once:

- `AutomationML_ObjectReferences_AttributeTypeLib_AMLEd2_1.1.1-beta.aml` (alias `ObjectReferences`) from the AML Editor library manager
- AutomationML Base Libraries, Edition 2, version 2.11.0 (referenced by URL)

## Notes

The FPD library is also part of the FPD–AML mapper, https://aml.fpbjs.net.

The libraries and the example belong to a manuscript submitted to *at – Automatisierungstechnik* (Nabizada, Drath, Ocker, Fay). Citation follows when it is out.
