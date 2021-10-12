# Data Mapping Table / ETL Definitions

Target Table XYZ [p.94]

| Target Field | Target Type | Len | Mandatory | Descr | Validation | Transformation/Navigation | Source Name   | Source Field |
|--------------|-------------|-----|-----------|-------|------------|---------------------------|---------------|--------------|
| ID           | int         |     | Y         | PK    | unique     |                           | sys generated |              |
| Type         | int         |     | Y         | Key   | must exist | link to user entered data in XYZ x-reference tbl... | XZY, XYZ-X-Ref | See Transformation |
| ...          | ...         | ... | ...       | ...   | ...        | ...                       | ...           | ...          |
