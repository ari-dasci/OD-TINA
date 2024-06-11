# Time-series Industrial Anomaly dataset

We present the **T**ime-series **In**dustrial **A**nomaly dataset (TiNA), a new time-series dataset for anomaly detection in an industrial context. The dataset contains the information from the sensor system of a mining machine owned by the company ArcelorMittal.

The TiNA dataset provides more than 38 million samples with 108 features in total. The time-step frequency is 2 seconds, therefore giving a range of 468 days from September 6th 2017 until December 25th 2018.

For publishing this dataset the dataset has been conveniently anonymized. More precisely all the numerical columns of the dataset have been normalized. The categorical columns have been also transformed, changing the category name to a different one to preserve the anonimity of the original data. The categorical columns of this dataset are the ones named "FEATURE76", "FEATURE87", "m_id", "m_subid" and "alarms". The variable "m_id" represents whether or not a maintenance has occured in that timestamp, identifying the type of maintenance by code. The "m_subid" variable identifies the subtype of maintenance if one has occured and the "alarms" column identifies alarm events. A maintenance is an operation which needs the machine to completely stop, therefore the normality is not reached instantly after the maintenance due to the recovery time of it. The alarms are events observed by the machinery operators which may or may not derive in a maintenance. The rest of the columns are all numerical. If the failure is detected and solved on the go the machine should continue functioning. The names of the columns have been changed and shuffled in order not to give information about the type of machine.



|                  | m_id | m_subid | alarms |
| ---------------- | ---- | ------- | ------ |
| Number of values |  15  |    7    |  155   |



There are 15 different types of maintenance codes, 7 subtypes of maintenances and 155 different alarms (counting in all the cases the none value).

- Maintenance codes: "none", "M1", "M2", "M3", "M4", "M5", "M6", "M7", "M8", "M9", "M10", "M11", "M12", "M13", "M14"

- Maintenance subid codes: "none", "MS1", "MS2", "MS3", "MS4", "MS5", "MS6"

- Alarm codes: "A1", "A2", "A3", "A4", "A5", "A6", "A7", "A8", "A9", "A10", "A11", "A12", "A13", "A14", "A15", "A16", "A17", "A18", "A19", "A20", "A21", "A22", "A23", "A24", "A25", "A26", "A27", "A28", "A29", "A30", "A31", "A32", "A33", "A34", "A35", "A36", "A37", "A38", "A39", "A40", "A41", "A42", "A43", "A44", "A45", "A46", "A47", "A48", "A49", "A50", "A51", "A52", "A53", "A54", "A55", "A56", "A57", "A58", "A59", "A60", "A61", "A62", "A63", "A64", "A65", "A66", "A67", "A68", "A69", "A70", "A71", "A72", "A73", "A74", "A75", "A76", "A77", "A78", "A79", "A80", "A81", "A82", "A83", "A84", "A85", "A86", "A87", "A88", "A89", "A90", "A91", "A92", "A93", "A94", "A95", "A96", "A97", "A98", "A99", "A100", "A101", "A102", "A103", "A104", "A105", "A106", "A107", "A108", "A109", "A110", "A111", "A112", "A113", "A114", "A115", "A116", "A117", "A118", "A119", "A120", "A121", "A122", "A123", "A124", "A125", "A126", "A127", "A128", "A129", "A130", "A131", "A132", "A133", "A134", "A135", "A136", "A137", "A138", "A139", "A140", "A141", "A142", "A143", "A144", "A145", "A146", "A147", "A148", "A149", "A150", "A151", "A152", "A153", "A154", "none"



|                  | Maintenances | Alarms  |
| ---------------- | ------------ | ------- |
| Number of events |   191,241    | 587,398 |



The total number of maintenances inside the dataset is 191,241 and the total number of alarms is 587,398.

## Citation

Please use the following citation:

```
@misc{tina_dasci_arcelor,
  title={Time-series Industrial Anomaly dataset},
  authors={Ignacio Aguilera-Martos and David López and Marta García-Barzana and Julián Luengo and Francisco Herrera},
  year={2022},
  URL={https://github.com/ari-dasci/OD-TINA}
}
```

## Contact

- Ignacio Aguilera Martos (nacheteam@ugr.es)
- David López Pretel (derwey@correo.ugr.es)
