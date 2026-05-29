# BingeBuddy: AI-Powered Movie Recommendation Platform

BingeBuddy is an intelligent movie recommendation platform that helps users discover movies tailored to their interests. Built using Machine Learning and content-based filtering techniques, it analyzes movie metadata from the TMDB dataset and generates personalized recommendations using cosine similarity.

---

## Features

* **Personalized Movie Recommendations:** Suggests movies based on content similarity and user interests.
* **Content-Based Filtering:** Uses cosine similarity to identify movies with similar characteristics.
* **TMDB Dataset Integration:** Trained on a large movie dataset containing genres, cast, keywords, and descriptions.
* **Fast Recommendation Engine:** Generates relevant recommendations in real time.
* **Movie Search:** Search and explore thousands of movies from the dataset.
* **Responsive User Interface:** Modern and intuitive design optimized for desktop and mobile devices.

---

## Project Structure

```bash
BingeBuddy/
├── frontend/      # Next.js client application
├── backend/       # Flask recommendation API
├── model/         # Trained ML model and preprocessing files
├── dataset/       # TMDB movie dataset
└── assets/        # Static resources
```

---

## Tech Stack

### Frontend

* **Framework:** Next.js
* **Styling:** Tailwind CSS
* **Language:** JavaScript

### Backend

* **Framework:** Flask
* **Language:** Python

### Machine Learning

* **Algorithm:** Content-Based Filtering
* **Similarity Metric:** Cosine Similarity
* **Dataset:** TMDB Movie Dataset
* **Libraries:** Pandas, NumPy, Scikit-learn

---

## Setup Instructions

### Prerequisites

* Python 3.9+
* Node.js 18+
* npm

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd BingeBuddy
```

### 2. Install Frontend Dependencies

```bash
cd frontend
npm install
```

### 3. Install Backend Dependencies

```bash
cd ../backend
pip install -r requirements.txt
```

### 4. Run the Backend Server

```bash
python app.py
```

### 5. Run the Frontend

```bash
cd ../frontend
npm run dev
```

Open:

```text
http://localhost:3000
```

to access the application.

---

## How the Project Functions

### 1. Data Processing

Movie metadata from the TMDB dataset is cleaned and preprocessed before training.

### 2. Feature Engineering

Genres, cast, crew, keywords, and movie descriptions are combined into feature vectors representing each movie.

### 3. Similarity Calculation

Cosine similarity is applied to measure the closeness between movie feature vectors.

### 4. Recommendation Generation

When a user selects a movie, the system identifies the most similar movies and returns ranked recommendations.

### 5. User Experience

The Next.js frontend communicates with the Flask backend and displays personalized recommendations through a responsive interface.

---

## Model Performance

* Achieved **87% recommendation accuracy**
* Trained on the **TMDB Movie Dataset**
* Generates highly relevant recommendations using movie content rather than popularity metrics
* Provides fast recommendation responses for a seamless user experience

---

## Deployment

### Frontend (Vercel)

* Connected to GitHub repository
* Automatic deployments on push
* Environment variables configured through Vercel dashboard

### Backend

* Flask API hosts the recommendation engine
* Serves recommendation requests and similarity calculations

---

## Dataset

The recommendation engine is trained using the **TMDB Movie Dataset**, which includes:

* Movie Titles
* Genres
* Cast Information
* Crew Information
* Keywords
* Movie Overviews
* Ratings and Metadata

---

## Future Enhancements

* User Authentication
* Personalized Watchlists
* Hybrid Recommendation System
* Collaborative Filtering
* User Rating System
* Trending and Popular Movie Sections
* Recommendation Explanation Features

---

## Contributing

Pull requests and suggestions are welcome. Feel free to open issues for bugs, feature requests, or improvements.
