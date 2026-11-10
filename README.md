# ExamDesk – Online Examination Platform

ExamDesk is a web-based online examination platform inspired by the computer-based examination interface of JEE Main. It allows students to attend scheduled examinations online using their roll numbers and provides administrators with facilities to manage students, examinations, and questions.

The platform has two user roles: **Admin** and **Student**.

## 1. Admin Module

The Admin is responsible for managing the examination system.

- Secure admin login.
- Import student details through CSV files.
- Manage student accounts using roll numbers.
- Manage branches, sections, semesters, and student groups.
- Create, update, and delete examinations.
- Configure examination names, instructions, schedules, and durations.
- Create and manage MCQ questions.
- Add four options to each question and specify the correct answer.
- Assign examinations to specific student groups.
- Configure examination questions and their order.

## 2. Student Module

Students access the platform using their assigned roll number and password.

- Secure student login.
- View assigned examinations.
- View examination instructions before starting.
- Start examinations when they are available.
- Attend examinations through a fullscreen interface.
- Navigate between questions using the question palette.
- Select one answer from four MCQ options.
- Move between questions using Previous and Save & Next.
- Clear selected responses.
- Mark questions for review.
- View the status of answered, unanswered, visited, and marked-for-review questions.
- Submit the examination manually or allow automatic submission when time expires.

## 3. Examination Interface

The examination interface follows the general design and navigation experience of the JEE Main computer-based test.

- All questions appear in one continuous sequence, from Q1 to Q20.
- Only one question is displayed at a time.
- A question navigation palette allows students to directly access any question.
- A countdown timer displays the remaining examination time.
- Students can navigate freely between questions.
- Responses are saved automatically.
- The interface requests fullscreen mode during the examination.
- Browser tab switching, switching away from the examination window, and exiting fullscreen are monitored as potential violations.

## 4. Examination Rules

| Parameter | Configuration |
|---|---|
| Total questions | 20 |
| Question format | Multiple Choice Questions |
| Options per question | 4 |
| Correct answers per question | 1 |
| Marks per question | 1 |
| Maximum marks | 20 |
| Negative marking | None |
| Question arrangement | Single continuous list |
| Examination timer | One timer for the entire examination |

### Violation Policy

The platform monitors examination violations.

1. **First violation:** Student receives a warning.
2. **Second violation:** Student receives a final warning.
3. **Third violation:** The examination attempt is automatically terminated and blocked.

Once blocked, the student cannot continue answering or submit further responses for that examination attempt.

## 5. Evaluation and Results

- Examination responses are automatically evaluated.
- Each correct answer receives one mark.
- Incorrect and unanswered questions receive zero marks.
- No negative marking is applied.
- The maximum possible score is 20.
- Results are displayed immediately after examination submission or automatic submission when the timer expires.
- Students can view their examination scores and results.

## 6. Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Java 25 |
| Backend Framework | Spring Boot |
| Authentication and Security | Spring Security, JWT |
| ORM | Spring Data JPA, Hibernate |
| Database | PostgreSQL |
| Frontend | React, TypeScript |
| UI Styling | Tailwind CSS |
| Testing | JUnit 5, Mockito |
| Deployment | Docker, AWS EC2 |

## Project Objective

To develop a secure, fullscreen, web-based examination platform that provides a JEE Main-inspired computer-based testing experience, supports CSV-based student management, enables administrators to conduct MCQ examinations, and automatically evaluates and displays student results.