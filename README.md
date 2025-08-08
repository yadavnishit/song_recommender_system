# Song_recommender_system

Song Recommender System (Based on Artist Name)
This project recommends songs by analyzing artist similarity. Enter an artist’s name, and it returns a list of songs from artists with similar musical style or metadata.

🎯 What It Does
Type in an artist name, and it suggests songs from other similar artists. It's a content-based filtering approach, working entirely from the metadata—no user data required.

🧠 How It Works
Dataset: Includes artist names, song titles, and other metadata (genres, features, etc.)

Preprocessing: Cleans and filters data to focus on relevant info (artist, song name, etc.)

Vectorization: Transforms artist names into numerical format using CountVectorizer

Similarity Matching: Uses cosine similarity to find similar artists

Recommendations: Fetches top N similar artists and returns some of their songs

🧰 Tech Stack
Python 3

Pandas

Scikit-learn

Jupyter Notebook

📂 Files
Untitled1.ipynb — Main notebook with the full implementation

songs_dataset.csv — Dataset (ensure it's available locally)

README.md — Project documentation (this file)

✅ How to Run
Download or clone the repo

Install the required packages:

bash
Copy
Edit
pip install pandas scikit-learn
Open the notebook:

bash
Copy
Edit
jupyter notebook Untitled1.ipynb
Scroll to the last cell and try:

python
Copy
Edit
recommend_songs_by_artist("Eminem")
It will return a list of songs from similar artists.

💡 Example Output
python
Copy
Edit
recommend_songs_by_artist("Eminem")
markdown
Copy
Edit
Recommended Songs:
1. Lose Yourself - 50 Cent  
2. Not Afraid - Lil Wayne  
3. Mockingbird - Dr. Dre  
4. Stan - Snoop Dogg  
5. The Real Slim Shady - Busta Rhymes  
(Output depends on actual dataset used. Placeholder example above.)

📌 Limitations
Works only with artists present in the dataset

Doesn’t account for user taste or song lyrics

Artist similarity is based on name/metadata, not actual music/audio features

📈 Future Ideas
Add audio features (e.g. tempo, energy) using Spotify API

Support user-based filtering and preferences

Deploy as a web app using Streamlit or Flask

🙌 Credits
Dataset sourced from [" https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023   "]
