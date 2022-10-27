## SUPER BOWL TV VIEWERS (0. README)

---

### 0.0 tl;dr

An end-to-end project that studies and creates a Machine Learning model to predict amount of Super Bowl TV Viewers.

---

### 0.1 PROJECT PURPOSE AND CONCEPTION

The Super Bowl is one of the world's biggest sports event each year. It is the climax of the NFL season and, probably the climax of the American Sports as well. 

No football fan (go, Cowboys!) misses the game, regardless if one's team is actually still a contender. That creates a lot of expectation and moves gigantic amounts of money on advertising, tickets, food, bets and many other things.

Not surprisingly, a Super Bowl ad with just a few seconds on TV might cost a few millions of dollars. And that is why this project will try to answer the question: "how many people will actually watch the game at home? 

---

### 0.2 DATA AND TOOLS USED

Two main datasets were used to create this project, even though a few others were also consulted. References to them can also be found on the notebook.

1. https://public.opendatasoft.com/explore/dataset/super-bowl/table/?sort=date&rows=60
2. https://www.sportsmediawatch.com/super-bowl-ratings-historical-viewership-chart-cbs-nbc-fox-abc/

This study used a Jupyter notebook as the main tool for development, while the documentation for some libraries used (such as Plotly) also came in handy.

---

### 0.3 SKILLS SHOWN

1. General Python coding;
2. "Real world" data collection, with the challenge of finding relevant data; 
3. Data cleaning and exploration, including the creation of a Map of Hypothesis;
4. Feature analyzis, engineering and selection;
5. Creation and comparison of Machine Learning models, based on few error metrics and model details;
6. Data visualizations with Seaborn and Plotly;
7. Basic concepts and commands of versionalization with git and integration with Github; _and_
8. DataFrame manipulation (pandas).

---

### 0.4 PREMISES

The only premise worth pointing out is that some of the features used for the model could only be account for _after_ the game (such as point difference) in real life, but here they are being considered as predictive.

---

### 0.5 PIPELINE (PROJECT PHASES)

![1 (1)](https://user-images.githubusercontent.com/108877184/182939648-c2b425e8-2354-4748-8c63-41f9c722cad6.jpg)

---

### 0.6 FURTHER DEVELOPMENT SUGGESTIONS

Ideas to build on top of this project and extend it.

1. The first iteration of this project counted with two steps that might have allowed data leakage. For the sake of "moving on", these mistakes were not changed, however, on a new iteration, they should be looked at. Feature normalization should only happen after the split between training and testing sets and the scaler should be fit to the training set only, to then transform both training and testing sets. Also, a random train_test_split with a time variable might also allow data leakage - [a simple time split validation could be useful](https://forecastegy.com/posts/3-essential-methods-to-do-time-series-validation-in-machine-learning/)
2. Add the data from the halftime show - use the number of artists and genres to create new data;
3. Adapt the data from 1967 to use it on the model;
4. Edit the column with the Year data, either encoding or normalizing it; _and_
5. Use nielsen ratings category for the model, instead of float numbers.
