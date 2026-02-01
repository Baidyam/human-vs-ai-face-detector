# Human vs AI Face Detector

An interactive game where humans compete against a deep learning model to identify AI-generated faces.

This project comes under Computer Vision and demonstrates the full ML lifecycle:
data exploration, model training, transfer learning, fine-tuning, evaluation, and deployment.

---

## What Does This App Do?

- Displays face images from a test set
- The user guesses whether the face is **Real** or **AI-Generated**
- A trained deep learning model makes its own prediction
- Human and model performance are compared in real time
- Scores and accuracy are tracked across multiple rounds

---

## Model Details

- **Architecture:** MobileNetV3 (Transfer Learning)
- **Training Strategy:**
  - Pre-trained on ImageNet
  - Custom classification head added
  - Top layers fine-tuned for better performance
- **Best Model:** Saved as `best_model.keras`
- **Evaluation Metrics:** Accuracy, validation curves, model comparison

---

## Game Features

- 10-Round Challenge: Complete game session with automatic ending
- Round Counter: Track your progress (e.g., Round 3/10)
- Live Scoring: Real-time accuracy comparison between Human and AI Model
- Instant Feedback: See the correct answer, your guess, and model's prediction with confidence score after each round
- Final Winner Declaration: Automatic performance summary and winner announcement after 10 rounds
- Restart Option: Start a new game session anytime with the Restart Game button
- Simple, Mobile-Friendly Interface: Clean Gradio UI that works on any device

---

## How to Use

1. Look at the displayed face image on screen
2. Make your guess by clicking either:
   -  Real button (if you think it's a real human face)
   -  AI-Generated button (if you think it's AI-created)
3. View the results which show:

   -  Correct answer (Real or AI)
   -  Your guess
   -  Model's guess with confidence score (0.00-1.00)
   -  Updated accuracy scores for both you and the model
4. Continue playing:
   -  Click Next Image to load the next face
   -  Complete all 10 rounds
5. See the final results:
   -  After Round 10, the game automatically declares the winner
   -  Compare your accuracy percentage vs the AI model
6. Play again: Click Restart Game to start a fresh 10-round session

---

## Tech Stack

- Python
- TensorFlow / Keras
- Gradio
- NumPy
- Pillow

---


---

## Notes

- The model runs on CPU (Hugging Face Spaces free tier)
- Predictions may take a second to load
- Images are preloaded for smooth gameplay

---

## Author

**Moumita Baidya**  
email: baidya.m@northeastern.edu

MS in Data Science  
Human vs AI Face Detection Project


