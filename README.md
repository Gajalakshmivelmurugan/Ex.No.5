# EXP 5: COMPARATIVE ANALYSIS OF DIFFERENT TYPES OF PROMPTING PATTERNS AND EXPLAIN WITH VARIOUS TEST SCENARIOS

# Aim: To test and compare how different pattern models respond to various prompts (broad or unstructured) versus basic prompts (clearer and more refined) across multiple scenarios.  Analyze the quality, accuracy, and depth of the generated responses 

### AI Tools Required: 
ChatGPT

## INTRODUCTION

Prompt engineering is the process of creating suitable instructions for an AI system. The quality of an AI response depends greatly on how clearly the user describes the required task.

A simple prompt gives limited instructions, while a structured prompt provides additional information such as the role, objective, audience, format, and restrictions.

<img width="950" height="537" alt="image" src="https://github.com/user-attachments/assets/ee82c095-3de1-407e-ae61-fb52f69a6175" />

## TYPES OF PROMPTS

## Simple Prompt

A simple prompt contains only the basic requirement and does not provide much information about the expected response.
## Example
```
Explain Machine Learning.
```
The AI decides the explanation level, format, examples, and length.

## Structured Prompt

A structured prompt provides clear instructions about what to explain, who the audience is, what points to include, and how the answer should be presented.

## Example:

```
Explain Machine Learning to a first-year college student.
Define Machine Learning, explain its three major types,
give two real-world applications, and mention two benefits
and two limitations. Use simple English and bullet points.

```

<img width="945" height="501" alt="image" src="https://github.com/user-attachments/assets/2e6e2dd6-a316-45ef-b261-1faa5732f58a" />

## COMPARATIVE TEST SCENARIOS

## Scenario 1 – Email Writing

## Simple Prompt

```
Write an email asking for leave.
```
## Structured Prompt

```
Write a polite leave request email to a college professor.
The student needs two days of leave due to a family function.
Keep the email professional and under 120 words.
Include a suitable subject and closing.

```
## Comparison

| Parameter    | Simple Prompt | Structured Prompt |
| ------------ | ------------- | ----------------- |
| Clarity      | Moderate      | High              |
| Relevance    | Good          | Very High         |
| Format       | General       | Professional      |
| Completeness | Limited       | High              |
| Usefulness   | Moderate      | High              |

Observation: The structured prompt produces a more suitable email because it specifies the recipient, reason, duration, tone, and length.

<img width="946" height="528" alt="image" src="https://github.com/user-attachments/assets/e6b48d1b-fd46-429a-a704-21e0c5646181" />

## Scenario 2 – Health and Fitness Advice

## Simple Prompt
```
Give me a fitness plan.
```
## Structured Prompt
```
Create a beginner-friendly 7-day fitness plan for a college student.
Include 30-minute daily activities such as walking, stretching,
and basic bodyweight exercises. Provide rest periods and keep
the plan simple and easy to follow.
```
## Comparison

| Parameter    | Simple Prompt | Structured Prompt |
| ------------ | ------------- | ----------------- |
| Quality      | Moderate      | High              |
| Specificity  | Low           | High              |
| Practicality | General       | Very High         |
| Organization | Low           | Excellent         |
| Usefulness   | Moderate      | High              |

Observation: The structured prompt gives a clear and actionable plan instead of general fitness advice.

<img width="452" height="663" alt="image" src="https://github.com/user-attachments/assets/46e6db0c-2c84-4c82-8763-a2ac61d0b06c" />

## Scenario 3 – Programming Problem

## Simple Prompt

```
Write a Python program for sorting.
```

## Structured Prompt

```
Write a Python program to sort a list of integers
using bubble sort. Explain the algorithm step by step,
show the program, and demonstrate it using the input
[5, 2, 8, 1, 3]. Keep the explanation beginner-friendly.
```
## Comparison

| Parameter          | Simple Prompt | Structured Prompt |
| ------------------ | ------------- | ----------------- |
| Accuracy           | Good          | High              |
| Explanation        | Limited       | Detailed          |
| Code Specification | Missing       | Clear             |
| Example            | Missing       | Included          |
| Learning Value     | Moderate      | High              |

Observation: The structured prompt gives both the required algorithm and a sample input, making the answer easier to understand.

<img width="681" height="643" alt="image" src="https://github.com/user-attachments/assets/bbb2cfda-9377-4adf-a617-655ac2806937" />

 ## Scenario 4 – Travel Planning

 ## Simple prompt

 ```
Plan a trip to Chennai.
```
## Structured Prompt

```
Create a 2-day Chennai travel plan for a college student.
Include major tourist places, approximate visit order,
food suggestions, and budget-friendly activities.
Present the plan in a table with morning, afternoon,
and evening sections.
```

## Comparison

| Parameter       | Simple Prompt | Structured Prompt |
| --------------- | ------------- | ----------------- |
| Relevance       | Moderate      | High              |
| Detail          | Limited       | Detailed          |
| Organization    | Basic         | Excellent         |
| Practicality    | Moderate      | Very High         |
| Personalization | Low           | High              |

Observation: The structured prompt creates a more useful itinerary because the duration, target user, budget, and format are specified.

<img width="947" height="502" alt="image" src="https://github.com/user-attachments/assets/c706f7e5-d0cb-4d63-97ff-6de40134d7a3" />

## Scenario 5 – Educational Explanation

## Simple Prompt
```
Explain blockchain.
```

## Structured Prompt
```
Explain blockchain technology to a beginner.
Start with a simple definition and explain blocks,
transactions, hashing, and decentralization.
Give one real-world example and use a simple analogy.
Keep the explanation within 300 words.
```
## Comparison

| Parameter         | Simple Prompt | Structured Prompt |
| ----------------- | ------------- | ----------------- |
| Clarity           | Moderate      | Excellent         |
| Technical Depth   | Basic         | Detailed          |
| Examples          | Variable      | Included          |
| Organization      | Simple        | Structured        |
| Beginner Friendly | Good          | Very High         |

Observation: The structured prompt provides a clearer educational explanation because it defines the required concepts and audience.

<img width="711" height="696" alt="image" src="https://github.com/user-attachments/assets/ed6bd887-0df3-41c0-a057-80914498b431" />

## PROMPT TEMPLATING TECHNIQUES

A prompt template is a reusable structure that combines fixed instructions and changing information.

## Fixed Template
```
Generate a student performance report.
```

## Variable Template
```
Student Name: {student_name}
Subject: {subject}
Mark: {mark}
Grade: {grade}
```

## Rule-Based Template
```
If mark >= 80:
    Generate an excellent performance message.

If mark >= 50:
    Generate a satisfactory performance message.

Otherwise:
    Generate an improvement message.
```
## Sequential Template
```
Student Data
     ↓
Performance Analysis
     ↓
Weak Areas
     ↓
Improvement Suggestions
     ↓
Final Report
```
<img width="942" height="562" alt="image" src="https://github.com/user-attachments/assets/40ff632b-6025-4b34-ae5c-5643e32559ef" />

## COMMAND PATTERN

The Command Pattern converts a request into an object. It separates the component that requests an operation from the component that performs it.

For an AI-based student reporting system:

Client → Invoker → Command → Receiver

Client: Provides student information
Invoker: Student management system
Command: Report generation request
Receiver: AI/LLM model

<img width="896" height="581" alt="image" src="https://github.com/user-attachments/assets/49ed821f-cc02-4dfe-89f0-b59acc4e7871" />

## COMPONENTS OF COMMAND PATTERN

| Component         | Function                         |
| ----------------- | -------------------------------- |
| Command Interface | Defines the operation            |
| Concrete Command  | Performs report-generation logic |
| Invoker           | Sends the request                |
| Receiver          | AI/LLM generates the response    |
| Client            | Provides data and configuration  |

## INTEGRATION OF PROMPT TEMPLATE WITH COMMAND PATTERN

Prompt templates can be combined with the Command Pattern to create a flexible AI-based student performance reporting system.

The system can select an appropriate prompt template and send it to the AI model through a command object.

<img width="683" height="461" alt="image" src="https://github.com/user-attachments/assets/d68fcb35-f901-4f31-afa9-b3446bbb0667" />

## WORKFLOW
```
Student Data
     ↓
Select Prompt Template
     ↓
Insert Student Information
     ↓
Create Command Object
     ↓
Send Prompt to AI
     ↓
AI Analyzes Data
     ↓
Generate Performance Report
     ↓
Display Report
```
## ENGINEERING SCENARIO – SMART PARKING SYSTEM

## Real-World Scenario

A busy shopping mall has limited parking spaces. Drivers spend a lot of time searching for available spaces.

An AI-based smart parking system can use cameras and sensors to detect available parking spaces and guide drivers.

The system should:

Detect available parking spaces
Count occupied spaces
Identify free spaces
Display parking availability
Guide drivers to free spaces
Update the information in real time

<img width="938" height="517" alt="image" src="https://github.com/user-attachments/assets/7e8d88e3-841d-4fd1-a5df-1ff1fbc0884a" />

## NAÏVE ENGINEERING PROMPT

```
Design an AI-based smart parking system.
```
## Expected Output
The AI may provide a general answer:
```
AI cameras and sensors can detect parking spaces
and show drivers where spaces are available.
```
## Observation

The answer does not clearly describe:

Hardware
Software
Architecture
Detection algorithm
Data processing
Testing

## REFINED ENGINEERING PROMPT

```
Act as an AI and IoT engineer.

Design an AI-based smart parking system for a shopping mall.

The system should use cameras and sensors to detect
occupied and available parking spaces.

Include:

1. Problem definition
2. Requirements
3. Hardware components
4. Software components
5. System architecture
6. Working principle
7. Parking detection algorithm
8. Decision-making process
9. Flowchart
10. Python simulation
11. Test cases
12. Expected results
13. Advantages
14. Limitations
15. Future enhancements
```

## EXPECTED OUTPUT FROM REFINED PROMPT

```
Problem
   ↓
Requirements
   ↓
Hardware & Software
   ↓
System Architecture
   ↓
Detection Algorithm
   ↓
Decision Process
   ↓
Flowchart
   ↓
Python Simulation
   ↓
Testing
   ↓
Final Report
```

## SYSTEM ARCHITECTURE

```
Parking Camera
      ↓
Vehicle Detection
      ↓
Space Detection
      ↓
Occupancy Analysis
      ↓
Available / Occupied
      ↓
AI Decision
      ↓
Parking Display
      ↓
Driver Guidance
```
<img width="572" height="577" alt="image" src="https://github.com/user-attachments/assets/5d0eba43-9ed7-4c61-bc0e-d4700ef28ca0" />

## WORKING PRINCIPLE

Cameras capture the parking area.
AI detects vehicles.
The system identifies occupied spaces.
Free spaces are calculated.
Parking availability is updated.
The available spaces are displayed.
Drivers are guided to free spaces.
The information is continuously updated.

## DECISION ALGORITHM

```
Detect Parking Area
       ↓
Detect Vehicle
       ↓
Is Space Occupied?
    ↙       ↘
  YES        NO
   ↓          ↓
Occupied    Available
   ↓          ↓
Update      Update
Status      Status
    \        /
     ↓      ↓
 Parking Display
```

## PYTHON SIMULATION
```
def parking_status(occupied, total):

    available = total - occupied

    if available == 0:
        return "Parking Full"

    elif available <= 2:
        return "Limited Spaces Available"

    else:
        return "Parking Available"


print(parking_status(10, 10))
print(parking_status(8, 10))
print(parking_status(4, 10))
```
## Expected Output
```
Parking Full
Limited Spaces Available
Parking Available
```
## TEST CASES

| Test Case | Total Spaces | Occupied | Expected Result   |
| --------- | -----------: | -------: | ----------------- |
| TC01      |           10 |       10 | Parking Full      |
| TC02      |           10 |        8 | Limited Spaces    |
| TC03      |           10 |        4 | Parking Available |
| TC04      |           20 |       20 | Parking Full      |
| TC05      |           20 |        5 | Parking Available |
| TC06      |           20 |       18 | Limited Spaces    |

## EVALUATION

| Parameter             | Simple Prompt | Refined Prompt |
| --------------------- | ------------- | -------------- |
| Problem Understanding | Basic         | Detailed       |
| Requirements          | Limited       | Clear          |
| Architecture          | Missing       | Included       |
| Algorithm             | General       | Defined        |
| Testing               | Missing       | Included       |
| Usefulness            | Low           | High           |

## CONCLUSION

The experiment demonstrates that prompt structure has a major effect on AI-generated responses. Simple prompts provide general answers, while refined prompts provide more detailed, organized, relevant, and useful solutions.

The smart parking scenario also shows that a carefully designed engineering prompt can guide AI to produce requirements, architecture, algorithms, simulation, and test cases.

## RESULT

The experiment was successfully completed. The comparison showed that refined prompts generate more structured, relevant, and complete responses than simple prompts, especially for complex engineering problems.
