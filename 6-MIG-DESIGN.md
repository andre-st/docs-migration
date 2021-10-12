# System Migration Design Specification

- partitioned by KBDA to make creation easier if necessary
- the whole of this deliverable must be consistent

## Data Migration Timetable With Check Points [p.173]

- develop timetable top down
- windows of opportunity from reviewing stage 2 sys retirement policies

## Data Migration Technical Specification [p.174]

- load program specs
- fallback unload program specs [p.177]
- transient data store specs
- legacy data store changes
- must match reqm and solution description in (already signed) system retirement policies
- non-functional spec [p.177]: servers, database or network capabilities of the mig plattform

## Stage 3 System Retirement Policies [p.178]

- with Data Transition Rules as required
- amendments to stage 1 and stage 2 policies

## Data Fallback Plan [p.108/177]

> Data fallback, in essence, is the reverse of a data migration. We are taking data from the new system and rewriting it to the Legacy Data Stores from which it came [p.109]

### Check Points [p.110]

> it is normal ... to proceed in a sequence of Key Business Data Area loads [p.110]

After each stage of the load we will pause and check against System Retirement Policy criteria: Meeting must decide if it is safe to proceed [p.111]
- or partial fallback as far as the previous Check Point (commonest)
- or full fallback (whole migration a failure)
- or continue under caution 
- do not switch to phased delivery


### Fallback Window [p.112]

