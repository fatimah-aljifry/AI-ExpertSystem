# AI-ExpertSystem
DHD Expert System (SNAP-IV Based)

A rule-based expert system built in Python that assesses ADHD symptoms using the SNAP-IV 18-item questionnaire.
This system is designed to assist teachers in identifying potential ADHD patterns and recommending next steps.

Overview

This project implements an interactive expert system using the experta library. It:

Asks 18 structured behavioral questions
Converts qualitative answers into numerical scores
Evaluates symptom severity
Provides a diagnostic impression and recommendation
 Features
Interactive command-line questionnaire
Rule-based reasoning system
Automatic scoring and classification
ADHD subtype detection:
Inattentive
Hyperactive/Impulsive
Combined
Clear, actionable recommendations

How It Works
1. Input Collection

The system asks 18 questions based on the SNAP-IV scale:

Q1–Q9 → Inattention
Q10–Q18 → Hyperactivity/Impulsivity

Each answer is mapped to a score:

Response	Score
Not at all	0
Just a little	1
Quite a bit	2
Very much	3
2. Rule-Based Engine

The system uses forward-chaining rules to:

Ask questions in sequence
Store responses as facts
Trigger evaluation when complete
3. Evaluation Logic
Calculates total scores for both domains
Classifies severity:
Not clinically significant
Mild
Moderate
Severe
4. Diagnosis Output

Example:

DIAGNOSIS RESULT
Possible ADHD — Combined Presentation
Recommendation: Recommend clinical assessment for ADHD.
🛠️ Tech Stack
Python
Experta (Rule-Based Engine)
 How to Run
1. Install dependencies
pip install experta
2. Run the program
python your_file_name.py
   Example Interaction
Q1: Often fails to give close attention...
Your answer: Quite a bit

Q2: Often has difficulty sustaining attention...
Your answer: Very much
Disclaimer:
This is not a medical diagnostic tool!
