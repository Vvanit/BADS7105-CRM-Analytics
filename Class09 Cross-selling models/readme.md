## Product recomendation (Cross-selling model)
Dataset: Customer Preference Survey.csv (in class survey)

https://github.com/Vvanit/BADS7105-CRM-Analytics/blob/a5f57619deca6f6ec488031611d1482bddda83a0/Class09%20Cross-selling%20models/Customer%20Preference%20Survey.csv

### Step
- Data cleansing
- Running Assosiation rule

### Rule selection
- Lift & confidence > 80 percentile
- Antecedents <=1 (Low occurence of long sequence)
- Consequents >=2
- Confidence <1 (unsurprise item recommend at confidence = 1)

### Result
![2021-12-18 00 41 12](https://user-images.githubusercontent.com/46345359/146585813-a92b9509-23f6-4d5d-bf96-0577fc44e102.png)
