🍽️ Restaurant Recommendation System
This project is a content-based restaurant recommendation system that suggests similar restaurants based on user preferences and selected restaurant features using cosine similarity.

📌 Features Used for Recommendations
Cuisine Preferences:

south_indian_or_not

north_indian_or_not

fast_food_or_not

street_food

biryani_or_not

bakery_or_not

Other Features:

average_price

rating

⚙️ How It Works
The dataset is preprocessed using Min-Max Scaling to normalize values.

A cosine similarity matrix is computed between all restaurant feature vectors.

Given a restaurant name, the system finds and recommends the top N most similar restaurants.

🗂️ Dataset
Make sure your CSV file indian_restaurants.csv has at least the following columns:

restaurant_name

location

south_indian_or_not

north_indian_or_not

fast_food_or_not

street_food

biryani_or_not

bakery_or_not

average_price

rating

✍️ Author
Prasanna Ganesan

📜 License
This project is open source and available under the MIT License.

