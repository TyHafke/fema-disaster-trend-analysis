# Data Provenance

## Dataset Information

- **Source:** Federal Emergency Management Agency (FEMA)
- **Dataset:** Disaster Declarations Summaries v2
- **Date Accessed:** June 2026
- **File Format:** CSV
- **Records:** 69,936
- **Variables:** 28
- **Latest Declaration Date:** June 16, 2026

[Access the Original FEMA Dataset](https://www.fema.gov/openfema-data-page/disaster-declarations-summaries-v2)

## Data Dictionary

| Variable | Description |
|---|---|
| `disasterNumber` | Unique disaster declaration identifier |
| `femaDeclarationString` | FEMA declaration reference |
| `fyDeclared` | Fiscal year of declaration |
| `incidentType` | Disaster or incident category |
| `declarationDate` | Date of federal declaration |
| `state` | State or territory associated with the declaration |
| `declarationType` | Federal declaration classification |

## Data Processing

The original CSV is preserved without modification. Data cleaning and processing are performed within the Python notebook.

- Repeated disaster declaration numbers are consolidated to prevent double counting.
- Declaration identifiers are checked for consistency.
- Incident types are grouped for visualization.
- Fiscal year 2026 is excluded because the dataset does not cover the complete fiscal year.

## Data Limitations

FEMA disaster declarations reflect federal administrative decisions and do not necessarily represent individual natural disaster events. Changes in declaration policies and reporting practices may influence historical trends.

## File

`DisasterDeclarationsSummaries.csv`

The included dataset is the original snapshot used for this project, ensuring reproducibility of the reported results.
