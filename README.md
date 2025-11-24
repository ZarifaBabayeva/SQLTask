# SQLTask
tasks related to SQL

TASK 1: Package for Data Validation

A package students_package1 was created with procedures to validate: -
Gender: must be ‘M’ or ‘F’. Otherwise returns error. - Age: must be
greater than or equal to 18. - Phone number: must match Azerbaijan
mobile format using regexp_like. Valid format: +994XXXXXXXXX. -
Automatic age calculation: Calculates age from date_of_birth and updates
the table.

TASK 2: Student Average Score Function

A function student_average_score: - Returns the average score of a
student. - If student does not exist → error “Tələbə tapılmadı”. - If
scores do not exist → error “Tələbənin nəticəsi tapılmadı”.

TASK 3: Archiving Failed Students

A procedure set_students_archieve: - Calculates average score. - If
average < 50: - Marks student as failed. - Inserts student exam data
into students_archieve. - Removes student from students_data.

A daily job at 09:00 calls this procedure automatically via
DBMS_SCHEDULER.

TASK 4: Report by City and Gender

A PL/SQL block using cursor: - Counts students grouped by city and
gender. - Prints formatted report with dbms_output.

TASK 5: Students Without Exam Results

set_imtahan_neticesi procedure: - Marks all students who do not exist in
exam_data as failed.

TASK 6: Updating Data from Excel (MERGE)

Uses MERGE to update students_data using rows from updated_data table.

TASK 7: Birth Season and Year Report

SQL query that: - Detects season (yaz, yay, payız, qış) using month. -
Groups by season and birth year. - Counts students per group.

TASK 8: Email Validation

Query to find invalid emails: - Email must contain both first name and
last name. - Invalid ones are selected.

This file documents all work done in the PL/SQL script.
