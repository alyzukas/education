# Education project
- **Author:** Alyssa Zukas 
- **Date:** October 25, 2025

---

## Project Overview

**Introduction:** This project addresses inequality of educational opportunity in U.S. high schools. Here we will focus on average student performance on the ACT or SAT exams that students take as part of the college application process. <br>

- **Objective:** The main goal of this project is to apply the data science methodology to analyze the relationship between `student performance on the ACT or SAT exams` and `socioecomoic factors`. <br>


- **Draft Problem Statement:** Is school performance associated with socioeconomic factors?

- **Final Problem Statement:** Does school geoassignment have a large effect on school performance?

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Sources:** 

    - EdGap Information (EdGap_data.xlsx)[https://github.com/alyzukas/education/blob/main/data/EdGap_data.xlsx]
    - School Information (ccd_sch_029_1617_w_1a_11212017.csv [https://github.com/alyzukas/education/blob/main/data/ccd_sch_029_1617_w_1a_11212017.csv]
    - Geographical Assignment (EDGE_GEOCODE_PUBLICSCH_1617.xlsx)[https://github.com/alyzukas/education/blob/main/data/EDGE_GEOCODE_PUBLICSCH_1617.xlsx]

## Description    

- **EdGap:** The 1st primary data set is the EdGap_data.xlsx data set from **EdGap.org**. This includes the school ID in respect to the values (percentages, amounts, etc) for the ACT/SAT exam scores and the five socioeconomic variables outside of locale classification. This will be denoted as `edgap_info`.

- **School Information:** The 2nd is a data set from the National Center for Education Statistics (NCES), displaying information about a large subset of schools. This includes the school ID, name, city, state, zip code, and several other characteristics of the school district in the year of 2016. This will be denoted as `school_info`.

- **Geographical Information:** The 3rd data set is also from National Center for Education Statistics (NCES), displaying the `locale code` in the year of 2016 for **public schools**. This is the geoassignment for that school depending on the schools Longitute and Lattitude geographical information. This code assignment will be used to give the school a locale classification that determines its geographic setting - **City, Subarb, Town, or Rural**. This will be denoted as `geo_info`.

    - These locale classification assignments follow the value distribution standard found in the [EDGE Geocode Tech Doc](https://nces.ed.gov/programs/edge/docs/EDGE_GEOCODE_PUBLIC_TECHDOC.pdf)


- **License:** N/A

---

## Analysis

Jupyter Lab and Notebook

---

## Results
Based off of the differing average exam scores for each geoassignment category, it is safe to assume that a schools geographical assignment **does** have an affect on school performance. But based off how little these averages differ, we cannot confidently support that geoassignment necessarily has a **strong** affect on school performance.

When analyzing the relationship of school performace and all socioeconmic variables, it appears that there are **other school variables that have stronger effects on school performace** than geographical assignment. Specifically - percentage of college education, percentage of students from married-couple families, and median income.


---

## Authors

- Your Name - [@alyzukas](https://github.com/alyzukas)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Tools/libraries used:
    -  pandas
    -  NumPy
    - matplotlib.pyplot
    - seaborns grid modeling
    - statsmodels.formula.api
    - statsmodels.api
- Tutorials or papers referenced: DATA 5100 Class modules
- Inspiration or collaborators: Dr Fischer
