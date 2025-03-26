# Math Meme Repair

## Overview
"Math Meme Repair" is a Generative AI project aimed at fixing incorrect viral math memes. Many social media posts contain incorrect math expressions due to misunderstandings of fundamental rules like PEMDAS, fractions, and exponentiation. This project fine-tunes a model to correct such errors and provide clear explanations.

## Features
- **Automatic Math Meme Correction:** Identifies incorrect math expressions and generates the correct versions.
- **Explanation Generation:** Provides step-by-step explanations of the corrections.
- **Error Rating System:** Generates humorous ratings for incorrect memes (e.g., "90% sass, 10% patience").

## Dataset
- Collected 20 incorrect math memes from social media.
- Examples include errors in order of operations (PEMDAS), exponentiation, and fractions.
- The dataset pairs incorrect expressions with correct answers and explanations.

## Model Architecture & Fine-Tuning
- **Base Model:** Transformer-based Sequence-to-Sequence (Seq2Seq) model.
- **Fine-Tuning:** The model was trained to map incorrect math expressions to their corrected forms and explanations.
- **Preprocessing:** Tokenization and normalization applied to math expressions.

## Installation & Setup
### Prerequisites
Ensure you have Python installed along with the required libraries:
```bash
pip install numpy pandas torch transformers streamlit
```

## Usage Instructions
1. **Upload an Incorrect Math Meme:** The model analyzes the input.
2. **Corrected Output:** It generates the correct expression and provides an explanation.
3. **Error Rating:** A humorous rating is displayed based on the mistake.

## Evaluation & Testing
- **Testing Approach:** Three new incorrect math memes were fed into the model.
- **Performance Check:** Verified whether the model correctly identified and explained mistakes.
- **Example:**
  ```
  Input: 8 ÷ 2(2+2) = ?
  Output: Correct answer is 16. PEMDAS rule applied: 8 ÷ 2(4) = 8 ÷ 8 = 16.
  ```

## Examples & Deliverables
- **Before/After Meme Example:**
  ```
  Wrong: 5^2 = 10  -->  Correct: 5^2 = 25
  ```
- **Humorous Error Rating:**
  ```
  "85% confusion, 15% confidence."
  ```

## Challenges & Future Improvements
### Challenges
- Understanding complex math mistakes that involve multiple operations.
- Generating explanations in a human-like, understandable way.

### Future Improvements
- Increase dataset size with diverse math mistakes.
- Improve explainability by integrating symbolic math reasoning.
- Deploy as a web service with an interactive UI.

## References
- Transformer-based Seq2Seq models
- PEMDAS order of operations
- AI for educational applications

## Results
![Math Meme Repair Screenshot](https://github.com/Muradhameed921/Math-Meme-Repair/blob/main/M1.png)
