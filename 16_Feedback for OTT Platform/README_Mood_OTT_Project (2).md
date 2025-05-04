# 🎬 Mood-Based OTT Recommendation System

## 🔍 Project Objective

This project aims to develop a **smart recommendation system for OTT platforms** that suggests content based on a user's current **emotional state**. Instead of relying solely on watch history or popularity, our system focuses on the **mood** of the user, detected through various input modalities.

## 💡 Key Features

- **Multimodal Emotion Detection**:
  - **Speech to Emotion**: Uses voice input to classify emotional tone.
  - **Text to Emotion**: Analyzes user text input to infer emotion.
  - **Video to Emotion**: (Optional extension) Uses facial expressions to detect mood.

- **Unified Mood Vector Representation**:
  - Detected emotions are converted into a vector format with **7 universal emotional categories**:
    - `angry`, `happy`, `sad`, `disgust`, `surprised`, `fear`, `neutral`

- **Content Recommendation**:
  - Movie descriptions from the **TMDB dataset** are converted into vector representations.
  - Using **similarity comparison**, we recommend movies that best align with the detected emotional vector of the user.

## ⚙️ How It Works

1. User provides an input (text, audio, or video).
2. The input is processed and classified into one of the 7 emotions.
3. The system compares this emotion vector with pre-processed vectors of movie descriptions.
4. Movies with the **highest similarity scores** are recommended.

## 📦 Data Sources

- **Emotion Datasets**:
  - Audio: RAVDESS (or similar)
  - Text: Pre-labeled emotional texts
  - Video: FER+ or similar datasets (optional)

- **Movie Metadata**:
  - TMDB (The Movie Database) dataset for movie descriptions and metadata

## 🔮 Future Enhancements

- Integrate user history for hybrid recommendations
- Use transformer models for more accurate emotion classification
- Support for real-time video-based mood tracking

## 🤝 Team Contribution

This project was collaboratively built with a focus on deep learning, natural language processing, audio processing, and vector-based recommendation systems.