# Mushroom Classification

This project uses a dataset containing descriptions of hypothetical samples of 23 species of gilled mushrooms from the families Agaricus and Lepiota, extracted from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. [Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification).

## Contents

- [Description](#description)
- [Dataset Information](#dataset-information)
- [Libraries Used](#libraries-used)
- [Data Exploration](#data-exploration)
- [Data Preparation](#data-preparation)
- [Models and Techniques](#models-and-techniques)
- [Performance Evaluation](#performance-evaluation)
- [Model Interpretation](#model-interpretation)
- [Contact](#contact)

## Description

The goal of this project is to classify mushrooms as either edible or poisonous based on their physical characteristics using various machine learning models. The project explores different models and techniques to improve classification accuracy and interpretability.

## Dataset Information

The dataset includes 23 species of mushrooms, with the following data recorded for each species:

- **class**: edible (e), poisonous (p)
- **cap-shape**: bell (b), conical (c), convex (x), flat (f), knobbed (k), sunken (s)
- **cap-surface**: fibrous (f), grooves (g), scaly (y), smooth (s)
- **cap-color**: brown (n), buff (b), cinnamon (c), gray (g), green (r), pink (p), purple (u), red (e), white (w), yellow (y)
- **bruises**: bruises (t), no (f)
- **odor**: almond (a), anise (l), creosote (c), fishy (y), foul (f), musty (m), none (n), pungent (p), spicy (s)
- **gill-attachment**: attached (a), descending (d), free (f), notched (n)
- **gill-spacing**: close (c), crowded (w), distant (d)
- **gill-size**: broad (b), narrow (n)
- **gill-color**: black (k), brown (n), buff (b), chocolate (h), gray (g), green (r), orange (o), pink (p), purple (u), red (e), white (w), yellow (y)
- **stalk-shape**: enlarging (e), tapering (t)
- **stalk-root**: bulbous (b), club (c), cup (u), equal (e), rhizomorphs (z), rooted (r), missing (?)
- **stalk-surface-above-ring**: fibrous (f), scaly (y), silky (k), smooth (s)
- **stalk-surface-below-ring**: fibrous (f), scaly (y), silky (k), smooth (s)
- **stalk-color-above-ring**: brown (n), buff (b), cinnamon (c), gray (g), orange (o), pink (p), red (e), white (w), yellow (y)
- **stalk-color-below-ring**: brown (n), buff (b), cinnamon (c), gray (g), orange (o), pink (p), red (e), white (w), yellow (y)
- **veil-type**: partial (p), universal (u)
- **veil-color**: brown (n), orange (o), white (w), yellow (y)
- **ring-number**: none (n), one (o), two (t)
- **ring-type**: cobwebby (c), evanescent (e), flaring (f), large (l), none (n), pendant (p), sheathing (s), zone (z)
- **spore-print-color**: black (k), brown (n), buff (b), chocolate (h), green (r), orange (o), purple (u), white (w), yellow (y)
- **population**: abundant (a), clustered (c), numerous (n), scattered (s), several (v), solitary (y)
- **habitat**: grasses (g), leaves (l), meadows (m), paths (p), urban (u), waste (w), woods (d)

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- sklearn

## Data Exploration

Initial data exploration includes examining the structure of the dataset, checking for missing values, performing preliminary data analysis, and analyzing the distribution of the features.

## Data Preparation

To prepare the data, the following steps were taken:

- The "class" column was removed from the features.
- Each column was encoded using a LabelEncoder to convert categorical values to numerical values.
- Multiple mappings_dict were created for each of the encoded attributes.
- The data was split into X and y, with X containing all attributes except "class", which was used as the target variable.
- StandardScaler was applied to X to standardize the data.

## Models and Techniques

The following models were used in this project:

1. Logistic Regression
2. Decision Tree
3. Tuned Decision Tree
4. Random Forest
5. Tuned Random Forest
6. Naive Bayes

## Performance Evaluation

The performance of the models was evaluated using various metrics, including AUC, sensitivity, and balanced accuracy.

## Model Interpretation

The models were interpreted using various techniques, including SHAP summary plots to visualize feature importance.

## Contact
If you have any questions or suggestions, you can contact me at radi2035@gmail.com.