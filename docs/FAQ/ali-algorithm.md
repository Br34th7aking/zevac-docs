# AI Algorithm

### How does an AI algorithm trained on other databases become applicable to my hospital?
Our base algorithm has been trained over 400,000 data points. Every time we implement the system in a new clinical setup the model is retrained with the local data, thus making the output relevant only to the local setup.
What all parameters are used to recommend antibiotics in Zevac?

### We currently take into account 3 types of parameters
Environment-related: Patients place of residence
Patient-related: Age, Gender, Comorbidities, Length of stay, Previous admissions
Hospital related: Ward, Care type


### How frequently does the Zevac algorithm get updated?

### How much data is needed for training the algorithm?

### Does the algorithm take into account the patient's previous hospitalization and conditions e.g. Allergy, previous culture report or any other longitudinal data of the patient?
If this information is available in the historical data it is taken into account