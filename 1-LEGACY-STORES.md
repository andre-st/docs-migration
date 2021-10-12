# Legacy Data Store Name XYZ

## Documentation

| Field                       | Comments [p.47]   |
|-----------------------------|-------------------|
| Data Store Name             | + (historical) synonyms if any [p.145]
| Business Area               | in which it is located
| Physical Location           | Place, Hardware
| Data Store Owner            | Who can authorize to decommission this store?
| Business Domain Expert      | Who can interprete the data (meaning)?
| Other Data Stakeholders     | Technical Data Ex., Programme Ex., Corp Data Architect, Audit/Regulatory Ex., Data Customer (External use) [p.30]
| Format                      | Oracle, Access, Excel, ... 
| Key_Business_Data_Area(s)   | one of max. 12 significant conceptual entities (data-centric demcomposition of the data migration project from the legacy data stores; points to missing links, manual re-keying, data gaps etc; _not:_ business functions, organizational boundaries, target systems modules)
| KBDA(s) Entities            | 
| Data Volumes                | table records count, entity records count
| Data Churn or Turnover      | volatile store (many updates) or rather static
| Data Quality                | impressionistic view, A1-D4 [p.49] 
| Field-by-Field Analysis     | ?
| Reason for Exclusion        | from the migration programme (if any reason)
| Usage                       | who uses the data store, what they use it for and how significant is it


## Retirement Policy

A System Retirement Policy is the specification and plan for how a Legacy Data Store will be decommissioned [p.50].

| Field                       | Comments [p.53]   |
|-----------------------------|-------------------|
| Data_Retention_Requirements | e.g., financial records to be retained for a given number of years
| Access Requirements         | 'just in case' or 24/7 [After retirement? Now? Already documented in Data Churn?]
| Aspects Not Replaced        | [p.54], might persist after new system impl.
| Signed off                  | Data Store Owner

- Data Transitional Rules [p.55] (temp. business operating procedures put in place to cope with disturbance caused by data migration itself): update data in two places, alternative data stores for certain items, look for orders before date X in store1 else store2, Data Freeze [p.56]
- Reassurance of Transfer Accuracy [p.51]
	- Audit trail (anything from a record of Control Totals to a backup-store of all the records at each stage of their progression through the migration process)
	- Control Total (count of the number of records being transfered, count in legacy and new system)
	- User Acceptance Tests
	
- What are their acceptance criteria? "How will you be certain, before we switch the new system on (and the old system off), that the data in it matches the reality as you experience it?" instead of "is this the number of stores in your company" or "Does this sample of customers have the right name and adress? [p.182]
