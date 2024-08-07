# The Open University Dashboard



## Summary

The open University is a fictional institution of learning. This report is intended to analyse her demographics, course participation and performance within a certain period of time (which is unspecified in the report). 


### Steps followed 

- Step 1 : The following SQL query was used to retrieve information on Student ID, Code module, Final result, Gender from the open university database.
![Screenshot 2024-08-07 171141](https://github.com/user-attachments/assets/b4eb3ca8-5479-4484-b871-424d52c7ee8f) 

- Step 2 : Information on Student ID, Count of students who unregistered a code presentation and Code Presentation were retrieved from the database using the following query.
![Screenshot 2024-08-07 173558](https://github.com/user-attachments/assets/4ef1ab5f-b066-460f-887a-0723ceb1ccee)

- Step 3: The following SQL query was used to retrieve information from the database as well
![Screenshot 2024-08-07 174324](https://github.com/user-attachments/assets/34ec6a04-1b8e-4c94-af0b-1f555ebf1bf2)

- Step 4: Results from these three queries were saved in .csv and first imported into power query. Power query editor was used to check that the data type for each column is adequate. Also, in the view tab, under Data preview section, "column distribution", "column quality" & "column profile" options were checked. Since by default, profile will Open only for 1000 rows, select "column profiling based on entire dataset".

- Step 5: The average score for each student ID on assessmentuni.csv was calculated using the 'Group by' feature on the transform menu.
![Screenshot 2024-08-07 175900](https://github.com/user-attachments/assets/a6342dfd-9703-4d40-b4c9-d2f08f381642)

- Step 6: After examining the data and cleaning as neccessary, all the tables were loaded into power BI desktop.
- Step 7: On the model view, all three tables were connected using a star schema.
- Step 8: Card visuals were used to visualize the total number of students, the numbers and code mode and code presentations, and the numbers of students that unregistered a code presentation.
![Screenshot 2024-08-07 181902](https://github.com/user-attachments/assets/a0af172a-65b5-44c8-b4a1-4feacfc802fc)

![Screenshot 2024-08-07 182043](https://github.com/user-attachments/assets/f8d68f0c-778b-45e9-840a-528e3b84de31)

![Screenshot 2024-08-07 182147](https://github.com/user-attachments/assets/9ce57682-04bb-40a7-bc74-b1e512dc61c9)

![Screenshot 2024-08-07 182305](https://github.com/user-attachments/assets/9507f3c6-e64a-4c36-83a0-9c55478b4cb3)

# Snapshot of Dashboard
![Screenshot 2024-08-07 182638](https://github.com/user-attachments/assets/4422b234-a2df-4c6c-bcee-aa0c5db53482)


# Insights

### [1] demographics
    1.1) Total number of Students = 28.785k
    1.1.1) Number of Males  = 15.046k
    1.1.2) Number of Females = 13.739k
    - Generally speaking, males constitute a greater population of the total students.

    1.2) Number of Students who unregistered Code presentation = 9.082k
    1.2.1) Number of Males = 4.927k
    1.2.1) Number of Females = 4.155k

    1.3) The BBB code module has more registered students than any other module.

### [2] Performance
    2.1) Overall, 9.53% of the total students had distinction, 39.06% had pass, 21.99% failed and 29.42% withdrew.
    2.2) While code module BBB had the highest student registration, code module EEE recorded the highest overall average score.

### [3] Code Presentation unregistered 
    3.1) Code presentation 2014J had the highest number of students who unregistered, as 3.21k students unregistered. This can be filtered through by code module.
