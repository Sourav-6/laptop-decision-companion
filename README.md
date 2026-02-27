# 🚀 Learning Path Decision Companion

A structured **Decision Companion System** that helps users choose the
most suitable technical learning path based on their goals, constraints,
and priorities.

This system evaluates multiple options against weighted criteria and
provides a ranked, explainable recommendation.

------------------------------------------------------------------------

## 📌 Problem Understanding

The assignment requires building a **Decision Companion System** that:

-   Accepts multiple options
-   Accepts weighted criteria
-   Evaluates options against criteria
-   Produces a ranked recommendation
-   Clearly explains why the recommendation was made
-   Does not rely entirely on AI
-   Is explainable (not a black box)

Instead of using the provided examples, this project solves:

> **Choosing the optimal technical learning path based on career goals
> and constraints.**

------------------------------------------------------------------------

## 🎯 Objective

Help users decide between learning paths such as:

-   Backend Developer\
-   Fullstack Developer\
-   Data Scientist\
-   ML Engineer\
-   DevOps Engineer\
-   Mobile App Developer\
-   Cloud Engineer\
-   Cybersecurity Analyst

Based on:

-   Job market demand\
-   Return on investment\
-   Learning difficulty\
-   Time required\
-   Resource availability

------------------------------------------------------------------------

## 🧠 Assumptions Made

1.  Each learning path can be evaluated numerically on predefined
    criteria.
2.  Users have different priorities (e.g., fast job vs high salary).
3.  Trade-offs are inevitable (e.g., high ROI often means higher
    difficulty).
4.  A weighted scoring model is sufficient for structured
    decision-making.
5.  Real-world complexity can be approximated using normalized scoring.

------------------------------------------------------------------------

## 🏗️ System Design

### 🔹 Architecture

    src/
     ├── main.py        → User interaction & flow control
     ├── loader.py      → Loads dataset
     ├── scorer.py      → Weighted scoring engine
     ├── explainer.py   → Generates explanation
    data/
     └── paths.json     → Learning path dataset

------------------------------------------------------------------------

## ⚙️ Decision Logic

### Step 1: User Profile Input

-   Weekly study hours
-   Budget
-   Risk tolerance

### Step 2: Priority Selection

User selects one of: - Get Job Quickly - High Salary Focus - Easy
Learning - Strong Foundation - Balanced

Each selection maps to predefined weights.

### Step 3: Score Calculation

Final Score = Σ (criterion_score × user_weight)

### Step 4: Ranking

Paths are sorted in descending order.

### Step 5: Explanation

The system explains: - Why the top option scored high - Which criteria
influenced the outcome

------------------------------------------------------------------------

## 🎛️ Features

✔ Multiple decision options\
✔ Weighted criteria\
✔ Ranked recommendation\
✔ Explainable reasoning\
✔ Manual selection mode\
✔ Modular architecture\
✔ Extendable dataset

------------------------------------------------------------------------

## 🧩 Design Decisions & Trade-offs

### CLI Instead of Web App

-   Focus on logic clarity.
-   Reduced UI complexity.

### Deterministic Model Instead of AI

-   Ensures explainability.
-   Avoids black-box behavior.

### Predefined Weight Profiles

-   Improves usability.
-   Reduces user friction.

### Static Dataset (JSON)

-   Easy to expand.
-   Human-readable.

------------------------------------------------------------------------

## ⚠️ Edge Cases Considered

-   Invalid menu inputs
-   Extremely low study hours
-   High ambition but low risk tolerance
-   Conflicting priorities
-   Manual mode bypassing recommendation engine

------------------------------------------------------------------------

## ▶️ How to Run the Project

1.  Clone the repository
2.  Navigate to the `src` folder
3.  Run:

```{=html}
<!-- -->
```
    python main.py

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Web interface (React/Flask)
-   API-based dynamic dataset
-   Visualization dashboard
-   Sensitivity analysis
-   Unit testing
-   AI-assisted explanation layer

------------------------------------------------------------------------

## 👨‍💻 Author

Sourav Vijay\
B.Tech Computer Science
