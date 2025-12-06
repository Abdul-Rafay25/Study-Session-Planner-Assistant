# UseCases.md

## Title: Use Cases for Study Session Planner Assistant

This document outlines the key use cases for the Study Session Planning Assistant MVP.

---

## **Use Case 1 — Create a Study Plan**

### **Actor:**  
University Student

### **Trigger:**  
The student wants to generate a 1–2 week study plan for an upcoming academic goal (exam, quiz, project milestone).

### **Preconditions:**  
- The student has a clear academic goal.  
- Topics/subtopics are known.  
- The student knows their available time slots per day.

### **Main Flow:**  
1. The student opens the system.  
2. The student enters their academic goal (e.g., “Midterm Exam”).  
3. The student enters topics and optionally marks difficulty levels.  
4. The student enters available time slots for each day.  
5. The system processes the information.  
6. The system generates a day-by-day study schedule.  
7. The system displays the final plan in a readable format.

### **Alternate Flows:**  
- **A1:** If the user does not enter difficulty for topics → default difficulty = normal.  
- **A2:** If the user enters time slots less than required → system adjusts by extending topics across more days.  
- **A3:** If data format is invalid → system prompts user to correct input.

---

## **Use Case 2 — Distribute Topics Across Available Days**

### **Actor:**  
Study Planning Algorithm (System)

### **Trigger:**  
User submits inputs and requests plan generation.

### **Preconditions:**  
- All required input fields are filled.  
- At least 7 days of planning window available.

### **Main Flow:**  
1. System breaks topics into smaller chunks.  
2. System assigns chunks into day-wise slots.  
3. System balances workload evenly.  
4. System schedules revision for difficult or high-priority topics.  
5. Final schedule is compiled.

### **Alternate Flows:**  
- **A1:** If workload cannot be balanced → system generates best effort output and warns user.  
- **A2:** If topics exceed total time availability → system suggests reducing topics or increasing days.

---

## **Use Case 3 — Review and Adjust Plan**

### **Actor:**  
University Student

### **Trigger:**  
The study plan is generated.

### **Preconditions:**  
- Study plan is successfully created by the system.

### **Main Flow:**  
1. The student reviews the full schedule.  
2. The student evaluates difficulty distribution.  
3. The student checks revision sessions.  
4. The student exports or saves the study plan.

### **Alternate Flows:**  
- **A1:** Student adjusts time slots → system regenerates the plan.  
- **A2:** Student modifies topic difficulty → system recalculates distribution.

---

## **High-Level System Design (Diagram)**

```
+-------------------------+
|       User Input        |
|  - Academic Goal        |
|  - Topics               |
|  - Difficulty Levels    |
|  - Daily Time Slots     |
+------------+------------+
             |
             v
+-------------------------+
|   Topic Processing      |
| - Break down topics     |
| - Prioritize difficult  |
+------------+------------+
             |
             v
+-------------------------+
|   Scheduling Engine     |
| - Allocate daily tasks  |
| - Balance workload      |
| - Add revision sessions |
+------------+------------+
             |
             v
+-------------------------+
|   Study Plan Output     |
| - Structured schedule   |
| - Revision reminders    |
+-------------------------+
```

---

## **Summary**
The use cases describe how the student interacts with the system and how the system transforms inputs into a realistic, balanced 1–2 week study plan. The goal is to provide clarity, structure, and motivation for students preparing for short-term academic goals.
