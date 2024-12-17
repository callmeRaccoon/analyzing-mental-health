# analyzing-mental-health
Using PostgreSQL flavor to analyze international student's mental health in Japan with different prospects.

# Analyzing Students' Mental Health

## Project Overview
This project analyzes how the length of stay impacts the mental health diagnostic scores of international students.

## Dataset
- **stay**: Length of stay in years  
- **todep**: PHQ-9 test (depression scores)  
- **tosc**: SCS test (social connectedness)  
- **toas**: ASISS test (acculturative stress)  

## SQL Analysis
- Filtered for `stay` values that are not NULL.  
- Included only "Inter" students from the `inter_dom` column.  
- Grouped results by `stay`.  
- Calculated:  
   - **COUNT**: Number of students per stay group  
   - **AVG**: Average mental health scores rounded to 2 decimals.  

## Results
1. Shorter stays (1-3 years) show higher stress and depression scores.  
2. Longer stays show improved social connection scores.

## Files
- `notebook.ipynb` → Full Jupyter Notebook.  
- `analyzing_students_mental_health.sql` → Clean SQL code.  
