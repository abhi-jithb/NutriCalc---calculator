# 🥗 NutriCalc— Instant Nutritional Metric & Macro Calculator

A responsive, client-side web application designed to compute Basal Metabolic Rate (BMR), Total Daily Energy Expenditure (TDEE), and targeted macronutrient distributions based on individual physiological metrics and fitness goals.

---

## 🎯 Overview

Tracking personal nutrition starts with understanding baseline energy demands. **QuickNutri** provides a streamlined, zero-friction interface for calculating daily caloric needs and macronutrient breakdowns (Proteins, Carbohydrates, and Fats) without requiring account sign-ups, external APIs, or complex setup.

---

## ✨ Features

- **Accurate Metabolic Estimations:** Implements the clinically validated **Mifflin-St Jeor Equation** to derive baseline metabolic energy expenditure (BMR).
- **Goal-Adaptive Targets:** Dynamically shifts caloric targets based on user objectives:
  - **Weight Maintenance:** Standard maintenance baseline adjusted for moderate activity.
  - **Healthy Fat Loss:** Controlled caloric deficit (-400 kcal/day).
  - **Lean Muscle Gain:** Controlled caloric surplus (+350 kcal/day).
- **Automated Macronutrient Partitioning:** Allocates target calories into practical daily gram targets:
  - **Protein:** 25% of total caloric intake (4 kcal/g).
  - **Carbohydrates:** 50% of total caloric intake (4 kcal/g).
  - **Healthy Fats:** 25% of total caloric intake (9 kcal/g).
- **Modern Glassmorphism UI:** Styled with a dark-mode theme, custom-styled dropdown selectors, ambient lighting effects, and responsive cards.
- **Zero Overhead:** Built purely with vanilla web standards—runs instantly in any browser with zero dependencies or backend latency.

---

## 📐 Mathematical Formulation

### 1. Basal Metabolic Rate (BMR)
Calculated using the **Mifflin-St Jeor Formula**:

$$\text{BMR} = 10 \times \text{Weight (kg)} + 6.25 \times \text{Height (cm)} - 5 \times \text{Age (years)} + 5$$

### 2. Maintenance & Adjusted Targets
Total baseline energy expenditure is scaled using a moderate activity multiplier:

$$\text{Base TDEE} = \text{BMR} \times 1.35$$

- **Fat Loss:** $\text{Target} = \text{Base TDEE} - 400\text{ kcal}$
- **Muscle Gain:** $\text{Target} = \text{Base TDEE} + 350\text{ kcal}$
- **Maintenance:** $\text{Target} = \text{Base TDEE}$

### 3. Gram Computations
- $\text{Protein (g)} = \frac{\text{Target Calories} \times 0.25}{4}$
- $\text{Carbohydrates (g)} = \frac{\text{Target Calories} \times 0.50}{4}$
- $\text{Fats (g)} = \frac{\text{Target Calories} \times 0.25}{9}$

---

## 🛠️ Tech Stack

- **HTML5:** Semantic form inputs and structured layout.
- **CSS3:** Custom CSS properties (variables), glassmorphism styling, flexbox/grid architecture, and custom dropdown styling.
- **JavaScript (ES6+):** Real-time mathematical evaluation and dynamic DOM updates.

---

## 🚀 Getting Started

### Local Setup
1. Clone the repository:
   ```bash
   git clone [https://github.com/Anusmrith/QuickNutri-Calculator.git](https://github.com/Anusmrith/QuickNutri-Calculator.git)
