# Development

## How to contribute a concept by composition from existing concepts (OEOX-concept) ?

**The following guidelines are in place until a GUI on the OEP is launched.**

| minimum required concept information | guideline                                                                                                                                                                                                                                                                                     | example                                                                                                                                |
|--------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| IRI                                  | Users with OEO contributer identifier (e.g. 0001) use their identifier when adding new concepts. E.g. First concept added : OEOX_00010001, Second concept added : OEOX_00010002. <br>Apply [this manual ](https://github.com/OpenEnergyPlatform/ontology/wiki/Numerical-Identifiers#how-to-change-your-settings)to configure IRI settings in Protégé.                                          | OEOX_00010002                                                                                                                          |
| labels                               | Try to match the label naming with the axiomatization. However, ensure it still describes the real world concept well.                                                                                                                                                                        | wind turbine space requirement                                                                                                         |
| axioms                               | **Only equivalent to axioms are allowed!** <br><br> Use the Protégé "Class expression editor" to axiomize an oeox-concept with already existing concepts from the OEO. Pay attention to use domain and ranges as specifically as possible. We start with concepts that are "information content entities". | 'specific space requirement' and ('quantity value of' some 'wind energy converting unit')                                              |
| definitions                          | The definition should keep the strucutre of the axiomatization but should be a more readable. Background: When the GUI is launched the definitions should be created from the aximatization and suggested to the user.                                                                        | A wind turbine space requirement is a specific space requirement that is a quantity value of one or more wind energy converting units. |
|                                      |                                                                                                                                                                                                                                                                                               |                                                                                                                                        |

## Workflow of adding a concept

1. Read the concept composition guideline above
1. In Protégé change your "Specified IRI:" to "`http://openenergy-platform.org/ontology/oeo-extended/`"
1. Commit your concept with IRI, label, axioms, definition to the a `feature` branch
1. When the `feature` branch is merged into `main`automatic checks are in place
   1. Check for dublicates in IRIs
