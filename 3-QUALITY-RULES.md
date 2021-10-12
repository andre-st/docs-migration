# Data Quality Rule 

> Data Quality Rules are a statement of the metrics that will be used to measure the quality of the data for each of the data sets under consideration, either at Legacy Data Store or Key Business Data Area Level, and the set of steps that will bring current data to the level where these metrics are met [p.59]. A mini-project in its own right […] For most of Stage 1 and Stage 2, DQRs will be the project's key controlling activities [p.152]

Types of Data Quality Rules [p.64]:
- Internal Consistency ("first-cut data quality rules")
- External Consistency (KBDA model, cleaned data mapable to new system? "second-cut DQR")
- Reality Check (corresponds to the real world) 

| Field                           | Comments [p.65]                |
|---------------------------------|--------------------------------|
| Key Business Data Area or Legacy Data Store | brief from the [legacy data store document](1-LEGACY-STORES.md) so that this can be read in isolation; in/out [p.65]
| Scope                           | Is it for a single aspect of the store, is it a "first-cut quality rule", just assessment or cleansing too? [p.65]
| Data Store Owner                | 
| Business Domain Expert          | 
| Other Contributors To This Rule | job, title, phone numbers, ...
| Qualitative Assessment          | [p.66]
| Quantitative Assessment         | [p.66]
| Data_Cleansing_Method_Statement | [p.67] brief to help Programme Expert planning (schedule, resources, ...)
| Mitigation Statements           | [p.68] ??
| Mitigation Tasks                | [p.69] ??
| Metrics                         | [p.70]

---
How:
- data gap analysis [p.78]
- Transient/Transitional Data Stores (..., cross-reference tables old_id:new_id [p.86])
- fix gaps/infer 1:m-mappings with existing (unofficial) (historical transactional) data (see Legacy Data Store catalogue) [p.80,87], 
- 'best guess' mapping now and update data sheet goes out on first maintenance visit [p.87]
- Single Cross Reference Table [p.89]
- Default to M:1 with exceptions [p.89]: 70% is 1:1, 25% is M:1, 5% needs decisions->default value->report created that allows the users to correct the system post implementation
- ...

> mixing of a bit of data preparation, a bit of error handling and record rejection at load time, with a bit of defaulting in valid values and a recovery exercise after the event [p.90, "Syncretistic option"]
