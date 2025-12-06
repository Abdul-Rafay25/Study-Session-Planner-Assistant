# ProblemStatement.md

## Title: Study Session Planner Assistant

## 1. Introduction & Problem Context
University, College or School students often set short-term academic goals such as preparing for an exam, completing a project milestone, or revising specific topics but fail to convert these goals into an actionable study plan. As a result, students experience last minute cramming, uneven workload distribution, burnout, and incomplete revision.

The difficulty lies not in identifying *what* needs to be studied, but *how to structure* the study time over the next 1–2 weeks in a realistic and organized way.

## 2. Primary Users
- University, College, School students from any field.
- Students who struggle with time management, planning, or balancing study sessions with their routine.

## 3. User Pain Points
- Short-term goals feel overwhelming because they are vague.
- Students cannot divide topics effectively within limited daily time slots.
- Workload becomes unbalanced, leading to burnout or missed topics.
- Revision for difficult topics is often ignored due to poor planning.

## 4. Goal of the MVP (Minimum Viable Product)
The system aims to convert a **short-term academic goal** into a **balanced 1–2 week study schedule**.

The MVP will:
1. Accept a short-term academic goal (exam, quiz, project milestone, etc.)
2. Accept a list of topics the student must prepare.
3. Accept the student’s available time slots for each day.
4. Generate a structured schedule assigning specific topics to specific days and sessions.
5. Balance the workload to avoid overloading any single day.
6. Include revision or extra time for difficult or priority topics.
7. Provide a simple, clear, and actionable plan the student can realistically follow.

## 5. Scope (What the System WILL Do)
- Parse user inputs: goal, topics, daily availability.
- Break topics into smaller study sessions.
- Distribute sessions over a 7–14 day period.
- Ensure balanced workload distribution.
- Allocate revision sessions, especially for difficult topics.
- Output a clean, readable study schedule in text form.

## 6. Out of Scope (NOT Included in MVP)
- No integration with Google Calendar or external APIs.
- No adaptive scheduling based on real-time progress.
- No reminders, notifications, or productivity analytics.
- No long-term planning beyond 2 weeks.
- No user login system or multi-user support.
- No advanced machine learning forecasting or recommendation systems.

## 7. Assumptions
- The user will provide clear topics or subtopics.
- A daily time availability of at least 30 minutes is assumed.
- The plan duration is fixed between 7–14 days.
- All inputs are text-based.
- The student will follow the schedule once it is generated.
- Only one study plan needs to be generated at a time.

## 8. Problem Statement Summary
Students often struggle to convert short-term academic intentions into concrete study plans. This system solves the problem by automatically generating a balanced, actionable, and realistic study schedule based on the student’s goals, topics, and available time. The assistant focuses on simplicity and practical usability, offering a structured plan that University students can easily follow to stay consistent and prepared.
