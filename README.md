# VAERS_Outcomes_Analysis-Modelling

This project is devoted to analyzing VAERS dataset of COVID-19 vaccination adverse events.  
VAERS_EDA.ipynb contains preprocessing and cleaning steps

## Objectives

- To present explorational data analysis in regard to social parameters (age, gender)
- To explore outomes (dead/no dead) in regard to age and gender
- To present the most common symptoms across all events

## Dataset

The dataset for this repo can be found [on Kaggle](https://www.kaggle.com/ayushggarg/covid19-vaccine-adverse-reactions).
It contains 890836 entries for 633063 unique cases. As the project is mainly focused on the analysis of cases, the duplicates were removed and only unique cases (first entry for each case) are taken into account.

The dataset contains 51 variables, but the current analysis focuses on AGE_YR (age), SEX (gender), DIED (outcome), SYMPTOM1, SYMPTOM2, SYMPTOM3, SYMPTOM4, SYMPTOM5 (symptoms) nad VAX_MANU (vaccine manufacturer).

### Results

- Sex distribution: the dataset mainly represent female population (68%)
![SEX distribution](https://user-images.githubusercontent.com/86741579/156522043-8b5bf335-5653-49d3-b52e-309224a437f3.png)
- Meidan age is 50 years, the cases are nearly normally distributed
![AGE distribution](https://user-images.githubusercontent.com/86741579/156523708-76ef74e0-d405-4416-b92a-3d2c4d02a5dd.png)
- The cases with outcome DIED=Yes are different in a way that median age is higher (75 years old) and men represent more than half (53%) of the cases in this group 
![Died AGE distribution](https://user-images.githubusercontent.com/86741579/156524403-c6bde5f4-2eba-4aed-97b2-98b4ba1bfa06.png)
![Died SEX distribution](https://user-images.githubusercontent.com/86741579/156524430-94b15c1d-fceb-4b8b-9f47-42a3cce3a2de.png)
-The most common symptoms are:
Headache     
Fatigue                    
Chills                     
Dizziness                  
Pain                    
Pyrexia                
Pain in extremity          
Nausea                 
Arthralgia        
Injection site pain

![Symptoms](https://user-images.githubusercontent.com/86741579/156524902-067023c6-234b-4c84-be00-9fc6eb1468f5.png)

The Tablleau dashbord for results can be found here: https://public.tableau.com/shared/MMK99QB9C?:display_count=n&:origin=viz_share_link. It also contains visuals for manufacturers and geographical data.

Thank you!
