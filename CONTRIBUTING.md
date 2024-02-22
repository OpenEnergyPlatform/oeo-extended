# Development

## How to contribute a concept by composition from existing concepts (oeox-concept) ?

**The following guidelines are in place until a GUI on the OEP is launched.**

|     | guideline |
|-----|-----------|
| IRI |   Users with OEO contributer identifier (e.g. 0001) use their identifier when adding new concepts. E.g. First concept added : oeox_00010001 | Second concept added : oeox_00010002        |
|   labels  |     Try to match the label naming with the axiomatization. However, ensure it still describes the real world concept well.     |
|   axioms  |     Use the Protégé "Class expression editor" to axiomize an oeox-concept with already existing concepts from the OEO. Pay attention to use domain and ranges as specifically as possible.      |
|  definitions   |    The definition should be a more readable version of the axiomatization.   |
|     |           |

## Workflow of adding a concept

1. Read the concept composition guideline above
1. Commeit your concept with IRI, label, axioms, definition to the dev branch
1. When the `dev` branch is merged into `main`automatic checks are in place
   1. Check for dublicates in IRIs
