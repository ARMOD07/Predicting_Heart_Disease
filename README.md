# Predicting_Heart_Disease
 
 # Cardiovascular Disease Prediction

## Introduction

The World Health Organization (WHO) estimates that 17.9 million people die from cardiovascular diseases (CVDs) every year.  
**L'Organisation mondiale de la santé (OMS)** estime que 17,9 millions de personnes meurent chaque année de maladies cardiovasculaires (MCV).

There are multiple risk factors that could contribute to CVD in an individual, such as unhealthy diet, lack of physical activity, or mental illness. Identifying these risk factors early on could help prevent many premature deaths.  
**Il existe de multiples facteurs de risque** qui pourraient contribuer aux maladies cardiovasculaires chez un individu, comme une mauvaise alimentation, le manque d'activité physique ou une maladie mentale. L’identification précoce de ces facteurs de risque pourrait contribuer à prévenir de nombreux décès prématurés.

We are working for an R&D company that focuses on providing healthcare solutions. The company has collected anonymized data from multiple hospitals on several patients. The dataset includes relevant information for each patient, such as their personal information and some medical data, including whether or not they have had heart disease before.  
**Nous travaillons pour une entreprise de R&D** qui se concentre sur la fourniture de solutions de santé. La société a collecté des données anonymisées auprès de plusieurs hôpitaux sur plusieurs patients. L'ensemble de données comprend des informations pertinentes pour chaque patient, telles que ses informations personnelles et certaines données médicales, notamment s'il a déjà eu ou non une maladie cardiaque.

We are tasked with using the dataset to accurately predict the likelihood of a new patient having heart disease in the future. The dataset has the following features:  
**Nous sommes chargés d’utiliser l’ensemble de données** pour prédire avec précision la probabilité qu’un nouveau patient souffre d’une maladie cardiaque à l’avenir. L'ensemble de données présente les caractéristiques suivantes :

## Dataset Features

- **Age**: age of the patient [years]  
  **Age** : âge du patient [années]
  
- **Sex**: sex of the patient [M: Male, F: Female]  
  **Sex** : sexe du patient [M : Homme, F : Femme]
  
- **ChestPainType**: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]  
  **ChestPainType** : type de douleur thoracique [TA : angine typique, ATA : angine atypique, NAP : douleur non angineuse, ASY : asymptomatique]
  
- **RestingBP**: resting blood pressure [mm Hg]  
  **RestingBP** : tension artérielle au repos [mm Hg]
  
- **Cholesterol**: serum cholesterol [mm/dl]  
  **Cholesterol** : cholestérol sérique [mm/dl]
  
- **FastingBS**: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]  
  **FastingBS** : glycémie à jeun [1 : si FastingBS > 120 mg/dl, 0 : sinon]
  
- **RestingECG**: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]  
  **RestingECG** : résultats de l'électrocardiogramme au repos [Normal : normal, ST : présentant une anomalie de l'onde ST-T (inversions de l'onde T et/ou élévation ou dépression ST > 0,05 mV), HVG : montrant une anomalie ventriculaire gauche probable ou certaine hypertrophie selon les critères d'Estes]
  
- **MaxHR**: maximum heart rate achieved [Numeric value between 60 and 202]  
  **MaxHR** : fréquence cardiaque maximale atteinte [Valeur numérique comprise entre 60 et 202]
  
- **ExerciseAngina**: exercise-induced angina [Y: Yes, N: No]  
  **ExerciseAngina** : angine induite par l'exercice [Y : Oui, N : Non]
  
- **Oldpeak**: oldpeak = ST [Numeric value measured in depression]  
  **Oldpeak** : oldpeak = ST [Valeur numérique mesurée en dépression]
  
- **ST_Slope**: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]  
  **ST_Slope** : la pente du segment ST de l'exercice de pointe [Up : ascendant, Flat : plat, Down : descendant]
  
- **HeartDisease**: output class [1: heart disease, 0: Normal]  
  **HeartDisease** : classe de sortie [1 : maladie cardiaque, 0 : Normal]

## Exploratory Data Analysis

Before we jump into building a model, let's conduct exploratory data analysis on the dataset.  
**Avant de nous lancer dans la création d'un modèle**, effectuons une analyse exploratoire des données sur l'ensemble de données.

Please note: For each step of the project, you are encouraged to add appropriate headers or subheaders and any discussions or explanations you see fit. It's always beneficial to have an appropriate structure for any project. It will help others clearly understand your work and will enhance your portfolio. It doesn't have to be perfect in any sense of the word. The goal should be to clarify your thought process for every step.  
**Veuillez noter** : Pour chaque étape du projet, nous vous encourageons à ajouter des en-têtes ou des sous-titres appropriés ainsi que toute discussion ou explication que vous jugez appropriée. Il est toujours bénéfique d'avoir une structure appropriée pour tout projet. Cela aidera les autres à comprendre clairement votre travail et améliorera votre portfolio. Il n’est pas nécessaire que ce soit parfait dans tous les sens du terme. L’objectif devrait être de clarifier votre processus de réflexion à chaque étape.


 
