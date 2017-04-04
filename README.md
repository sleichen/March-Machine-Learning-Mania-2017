# March Machine Learning Mania 2017
This was a competition on Kaggle.com to successfully predict the outcomes of the 2017 NCAA Basketball Tournament. All of the data I used, as well as my submissions, are in the .csv files. The Jupyter notebook gives the actual model, and is meant to be readable. I used Python (mostly pandas and sklearn) to do the analysis.

This was my first real project in data science, and as such there's nothing too sophisticated. I ended up finishing 198/442, with a LogLoss of 0.515497. That's right in line with my expectations based on testing, and overall I'm happy with it. I've also got some things to keep in mind for next year:

1) Take the tournament structure into account. To some extent this is already implicit in the seed data, but I think more can be done with it. This could make an especially big difference once we get to the Final Four, which are the most inherently uncertain games to predict.

2) There are surely smarter things to do with the basic game statistics than just take averages oer the season. I saw one suggestion on the message board to use regression to extract values for (at least some of) the game statistics. That would account for upward or downward trends over the season better than a straight average.

3) New variables. There are a lot of variables that I didn't make use of. People on the message boards suggested that game location was important. Also there are sophisticated variables that one can construct, like an Elo rating, which could then be fed in to a neural net or something.

4) Better modeling. I just used the most basic MLP neural network because that's what I knew how to do. By next year I'll have a better understanding of what kinds of models work best for this problem, and I'll also know which packages to use for more sophisticated model building.
