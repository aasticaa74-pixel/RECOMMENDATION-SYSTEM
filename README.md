movies = {
    "Avatar": ["Titanic", "Interstellar", "Gravity"],
    "Titanic": ["Avatar", "The Notebook", "A Walk to Remember"],
    "Interstellar": ["Gravity", "Inception", "Avatar"],
    "Inception": ["Interstellar", "The Matrix", "Gravity"],
    "The Matrix": ["Inception", "Avatar", "Interstellar"]
}

print("=== Movie Recommendation System ===")
print("Available movies:")
for movie in movies:
    print("-", movie)

user_movie = input("\nEnter your favorite movie: ")

if user_movie in movies:
    print("\nRecommended movies for you:")
    for recommendation in movies[user_movie]:
        print("-", recommendation)
else:
    print("Sorry! Movie not found in the database.")
