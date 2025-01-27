# Music Recommendation System

This repository contains a Python-based Music Recommendation System that uses machine learning techniques to recommend songs similar to a given track. The system processes a dataset of songs, computes similarity metrics, and provides tailored recommendations.

---

## Features
- **Track Recommendations**: Recommends similar tracks based on cosine similarity.
- **Data Normalization**: Scales numerical features for improved similarity computations.
- **Customizability**: Adjustable sample size for processing large datasets efficiently.
- **Error Handling**: Includes validations to ensure robust execution.

---

## Prerequisites

Ensure you have the following installed:

- Python 3.8 or later
- Required libraries:
  ```bash
  pip install pandas numpy scikit-learn
  ```

---

## Dataset
The system uses a dataset containing the following columns:
- `track_id`
- `artists`
- `album_name`
- `track_name`
- `track_genre`
- Numerical features such as `popularity`, `duration_ms`, `danceability`, `energy`, etc.


---

## Usage

### 1. Clone the Repository
```bash
git clone https://github.com/NASO7Y/Music-Recommendation-System.git
cd Music-Recommendation-System
```

### 2. Run the Script

Ensure your dataset is placed in the correct directory and execute the script:
```bash
python recommend.py
```

### 3. Example Output
The script will recommend songs similar to a given track. Example:
```
Recommended Songs:
   popularity  duration_ms  danceability  energy  loudness  ...
0        0.89        0.75          0.87    0.93      0.71  ...
1        0.85        0.71          0.89    0.91      0.68  ...
...
```

---

## Functions

### `recommend_songs(track_index, num_recommendations=5)`
**Description**: Recommends songs similar to the track at the given index.
- **Parameters**:
  - `track_index` (int): Index of the track in the dataset.
  - `num_recommendations` (int): Number of recommendations to return.
- **Returns**: A DataFrame with recommended tracks.

### Example:
```python
recommended_songs = recommend_songs(0, num_recommendations=5)
print(recommended_songs)
```


---


## This project is made for CodeAlpha Training 

---
## Contact

GitHub: naso7y

Email: ahmed.noshy2004@gmail.com

LinkedIn: [LinkedIn](https://www.linkedin.com/in/nos7y/)