Database-model-for-education-portal

There are five individual tables as follows: 
    # students - containing student ids and student names
    # courses - containing course ids and course names
    # tasks - containing task ids, task details and expected submission date.
    # queries - containing query ids and details
    # teachers - containing teacher ids and teacher names.

Then there are tables with following relations: 
    # student_teachers_courses - containg student details taking up specific courses and the teachers allotted to teach the courses (all related by their respective ids)
    # courses_tasks - containing tasks pertaining to the courses (related by course and task ids)
    # courses_queries - containing queries under each course (related by query and course ids)
    # tasks_queries - containing queries based on each task (related by task  and course ids)
    # students_tasks - containing students and the tasks they have taken up with columns to hold actual date of submission of the task and corresponding score (related by student and task ids)
    # students_teachers_queries - containing students, with the corresponding queries raised by them and the teachers assigned to help with the queries. It also has the status of the queries (related by student, query and teacher ids)
    # students_mentors_list - containing students and their corresponding mentors (related by student and teacher ids)
