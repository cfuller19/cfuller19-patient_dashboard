# Patient Readmission Dashboard

<b> This is a tableau dashboard I created showing trends in hospital patient readmission by state. The dashboard can be filtered based on:
- initial admission method
- initial hospitalization length
- number of visits by the primary doctor during the initial hospitalization
- main hospital service provided
- state
- readmission status </b>

https://public.tableau.com/app/profile/courtney.fuller1893/viz/PatientReadmissionDashboard_17044112502620/PatientReadmission?publish=yes <br>
<img width="747" alt="image" src="https://github.com/cfuller19/cfuller19-patient_dashboard/assets/101231073/807d76a5-8e8e-46cf-bafe-a7a2bdc773f5"> <br>

Two data sources were used to create this dashboard. The first data source consisted of fictitious patient information from a hospital system in the United States. The second data set, obtained from Kaggle, summarizes data from the Centers for Medicare and Medicaid Services and provides readmission percentages per state between 2012 and 2020.<br><br>
The purpose of this dashboard is to provide insight to hospital executives on (1) current readmission rates compared to national averages of all hospital systems, and (2) trends that could contribute towards higher readmission rates. The overall trend observed from this dashboard is that a patient's experience during their initial hospitalization impacts their likelihood of hospital readmission within one month, and this experience differs state by state. For example, all patients who were readmitted to the hospital had initial hospitalization lengths of 50 days or more. Likewise, DC had the highest readmission rate of 46.15% while NH had the lowest readmission rate of 26.58%.<br><br>
The dashboard itself was designed to be accessible to people of diverse abilities by utilizing the following characteristics:
- a consistent, easy-to-read font was chosen for all visualizations
- a sans serif font was used to make letters appear less crowded
- bold text was used for emphasis
- larger font size was used for headings
- the dashboard is organized by category to keep it clean and remove unnecessary complexity
- the same color palette is used throughout to maintain a clean, cohesive appearance
- the "colorblind" palette on Tableau was chosen, where possible, for visualizations.
- the main color schemes utilized shades of blue, orange, and gray.
- all visualizations are supported with detailed tooltips providing the same information in text format to offer an alternative option to color for distinguishing data
- straightforward language and expression of data were used. <br>
<br>
<br>
<b> This is a second, similar dashboard I created exploring relationships between hospital rating and readmission rates within the fictitious hospital system in the United States.</b><br>
<br>Data used for this dashboard were obtained from 2 different sources: a medical_data database provided by Western Governors University, and accessed through pgAdmin (PostgreSQL), and an add-on csv file obtained from Kaggle.com.<br>
The add-on csv was added to the medical_data database after it had been cleaned to remove unnecessary columns and records containing null values.<br><br>
a.	To create the dashboard, first the add on csv was loaded into the medical_data database using pgAdmin/PostgreSQL. A create table script was written designating the name of each column in the table, along with the appropriate data type. Then the csv was imported into the table using the table’s menu. Then, within the ERD, the new table, hospital_general_info was related to the location table through the zip code columns.
b.	Within Tableau, only 3 tables from the database were needed to create the dashboard: the patient table, location table, and hospital_general_info table. The location table was inner-joined on the patient table. The hospital_general_info table was inner-joined on the location table. The SQL scripts used for this process can be examined in Tableau.<br>
https://public.tableau.com/app/profile/courtney.fuller1893/viz/HospitalReadmissionRatesByMetric/ReadmissionDashboard?publish=yes <br>
<img width="747" alt="image" src="https://github.com/cfuller19/cfuller19-patient_dashboard/assets/101231073/863790af-d06a-4f2f-b246-e774496410c7">



