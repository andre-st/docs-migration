# Issues

## Essential Prerequisites
- [x] enterprise no passive role: make everything a business not a technical problem
- [x] an open door policy to Legacy Data Stores
- [x] a virtual team of Data Stakeholders
- ... 


## Data Migration Impl.

- sequencing [p.99]: static/master data (low churn rate) first, volatile/tx data later, load some in parallel (scheduling/runtime); "it is normal ... to proceed in a sequence of Key Business Data Area loads" [p.110]: Location->Equipment->... climbs dependency hierarch.)
- windows of opportunity [p.101]: holidays, long weekends; you have to know migr. runtime: data extraction, data prep., data cleansing, bridging data gaps, data loads etc
- impl forms [p.103]
  - big bang impl (on the night, LDS switched off), cheap & high-risk -> fallback strategy [p.108]
  - parallel running impl (legacy stores continue to operate until lds owners satisfied that new sys is a success), most expensive & least-risk
  - phased delivery (incrementally, eg region by region), if too small opp-window, very large scale projects; doesnt save money or lower risks (adds risks: moving target)
 - pilot impl. [p.107] prior the big event: check timings, software, data trans rules, fallbacks (do not call it final testing phase or lose face)
 - 
- sign-offs [documents table p.179]

## Data Migration Testing [p.180]
- use ETL defs 
- use sys retirement policies (what stakeholders consider important, how to measure)
- 

## Data Mig Execution [p.183]
- risk register for any items that have not been completed and get store owners to sign off mitigation steps in the sys retirement policies [p.184] 
