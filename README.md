# GenreFinder

GenreFinder is an iOS app that tries to guess the genre of movies based on a description inputed by the user. The algorithm at the core of the app works on the premise that genres exist in a spectrum rather than in definite categories. Therefore when querying the app, the user is returned a list of genres ordered by probability of correspondence.

The artificial intelligence powering the app uses data from a list of 4456 movies (commandeered) from IMDB. Each entry in the data set contains a movie’s description and its corresponding three genres. While gathering a larger dataset was possible and would have improved the accuracy of the algorithm, it would also have made it extremely slow. Thus instead a library of synonyms is used to augment queries on this database.

The AI is a basic machine learning algorithm that associates individual and groups of adjectives, nouns, and adverbs with movie genres and weights them according to their occurrence in the dataset. Again a tradeoff exists between the accuracy of the algorithm and its running time and thus it is dumbed down a little to make it usable in an app.

On testing it is evident that this method of classifying movies has clear limitations as the algorithm is not truly able to infer meaning from user input. The resultant app is more of a playful experiment that demonstrates the difficulty in classifying movies.
