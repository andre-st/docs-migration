# Key Business Data Areas

- Entity Relationship Model
- using _conceptual_ entity models to define the key business data areas [p.41] [This is the highest level ER model; sowas wie logisches UML-Paketdiagramm]
  > A Conceptual Entity Model is a form of data model where atomic entities are grouped 
  > together to form higher-level entities that are meaningful to the enterprise [p.42]
- usually no more than 12 such entities
- from Legacy Data Stores
- data-centric decomposition, not business functions, organizational boundaries, target system modules
- the data models we are creating here are the data models of how the legacy KBDA should be structured, we expect that individual Legacy Data Stores will conform to this model to a greater or lesser degree [p.145f]
- where there is more than one LDS then a synthesis of their data structures will be required [p.146]
- beware academic correctness here; we are after a reasonable standard against which local divergence can be measured; differences betw. indiv. LDS and the KBDA model [p.146]
- we need our LDSs sufficiently consistent with the legacy KBDA models to allow the project to move forward to the 2nd stage of data prep. [p.147]

