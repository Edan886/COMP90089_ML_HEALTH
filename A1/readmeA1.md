**Feedback:**
1. One main disadvantage of mapping is, when we map from a high-resolution terminology like SNOMED-CT to a lower resolution terminology, like ICD codes, then we may loose some information. For example, to where ‘Low blood pressure reading’ in SNOMED CT will map in ICD codes? ‘Low blood pressure reading’ is one of the findings in the tree of ‘Hypertension’ in SNOMED-CT. Where can we map it in the ICD codes? We don’t know whether it is ‘Idiopathic’, or ‘Orthostatic’, or ‘hypotension due to drugs’, or ‘other hypotension’, or ‘hypotension, unspecified’, because we don’t have more information in ICD codes. 
2. It's better to use table 'emar' for medical administrations, rather than using 'inputevents' or 'prescriptions' table. If 'inputevents' table is used, should check 'statusdescriptions' column to filter successful administrations. When use 'emar' table, please pay attention to the 'event_txt' column. Not all the records in 'emar' represents successful administrations.


**FINAL MARK**:11.7/15
