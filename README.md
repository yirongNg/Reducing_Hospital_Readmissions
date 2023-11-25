# Reducing Hospital Readmissions

## 🔗 Project Links
- [Data Manipulation with SQL](https://app.datacamp.com/workspace/w/fbd56db5-1a00-4e5e-a86c-9b1585b47307)
- [Interactive Dashboard on Tableau](https://public.tableau.com/views/ReducingHospitalReadmissions/Story1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

## 📖 Background
You work for a consulting company helping a hospital group better understand patient readmissions. The hospital gave you access to ten years of information on patients readmitted to the hospital after being discharged. The doctors want you to assess if initial diagnoses, number of procedures, or other variables could help them better understand the probability of readmission. 

They want to focus follow-up calls and attention on those patients with a higher probability of readmission.

## 💾 The data

You have access to ten years of patient information ([source](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008)):

#### Information in the file
- "age" - age bracket of the patient
- "time_in_hospital" - days (from 1 to 14)
- "n_procedures" - number of procedures performed during the hospital stay
- "n_lab_procedures" - number of laboratory procedures performed during the hospital stay
- "n_medications" - number of medications administered during the hospital stay
- "n_outpatient" - number of outpatient visits in the year before a hospital stay
- "n_inpatient" - number of inpatient visits in the year before the hospital stay
- "n_emergency" - number of visits to the emergency room in the year before the hospital stay
- "medical_specialty" - the specialty of the admitting physician
- "diag_1" - primary diagnosis (Circulatory, Respiratory, Digestive, etc.)
- "diag_2" - secondary diagnosis
- "diag_3" - additional secondary diagnosis
- "glucose_test" - whether the glucose serum came out as high (> 200), normal, or not performed
- "A1Ctest" - whether the A1C level of the patient came out as high (> 7%), normal, or not performed
- "change" - whether there was a change in the diabetes medication ('yes' or 'no')
- "diabetes_med" - whether a diabetes medication was prescribed ('yes' or 'no')
- "readmitted" - if the patient was readmitted at the hospital ('yes' or 'no') 

***Acknowledgments**: Beata Strack, Jonathan P. DeShazo, Chris Gennings, Juan L. Olmo, Sebastian Ventura, Krzysztof J. Cios, and John N. Clore, "Impact of HbA1c Measurement on Hospital Readmission Rates: Analysis of 70,000 Clinical Database Patient Records," BioMed Research International, vol. 2014, Article ID 781670, 11 pages, 2014.*

## 🔍 Findings & Recommendations

1. The most common primary diagnosis for age group 40-50 is "Other Diagnosis" but "Circulatory Diagnosis" is common for age groups 50-60, 60-70, 70-80, 80-90, and 90-100. Patients above 50 years old who are diagnosed with circulatory issue have 55-70& chance of readmission. Therefore, doctors should perform more diagnostic tests and prescribed ideal treatments for these senior patients.

2. The top 3 groups of patient with high probability of readmission are diagnosed with Other (64%), Circulatory (62%), and Diabetes (35%). Among the patients who are diagnosed with other issues, 49% of them has circulatory problems and 31% of them has diabetes.

3. Patients who have zero outpatient visit before hospital stay is likely to have high readmission rate. Among the number of readmitted patient who has zero outpatient visit before hospital stay, 63% of them has other diagnosis and 62% of them has circulatory diagnosis.

4. About 56% of the readmitted patients do not have inpatient visit before hospital stay and 85% of the readmitted patients do not have emergency visit in a year before hospital stay. Thus, these two factors do not contribute to hospital readmissions.

5. About 50% of the total readmissions do not include the medical specialty of the doctor. Thus, there is a lack of data to find out which medical specialty administered patients' readmissions.

6. Among the 35% of readmitted diabetic patients, 92% of them did not do glucose test, 80% of them did not do A1C test, and 82% of them has diabetic medicine prescription by medical doctors. But since the medical specialty of the doctors was not administered in 50% of the total readmissions, it is not possible to investigate which medical specialty prescribes diabetic medication to patients.

![Story 1](https://github.com/yirongNg/Reducing_Hospital_Readmissions/assets/132359604/a044144c-4d83-4295-bbf1-4b3d9610cf4e)

![Story 1 (1)](https://github.com/yirongNg/Reducing_Hospital_Readmissions/assets/132359604/c4388ce1-323c-40e3-9094-5c9d63adde4e)



