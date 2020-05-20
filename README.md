# PetFinder.my-Adoption-Prediction
Objective : The purpose of this project was to predict the speed at which a pet is adopted, based on the pet’s listing on PetFinder. 

Data : The data included text, tabular, and image data

File descriptions
train.csv - Tabular/text data for the training set

test.csv - Tabular/text data for the test set

sample_submission.csv - A sample submission file in the correct format

breed_labels.csv - Contains Type, and BreedName for each BreedID. Type 1 is dog, 2 is cat.

color_labels.csv - Contains ColorName for each ColorID

state_labels.csv - Contains StateName for each StateID

AdoptionSpeed
Contestants are required to predict this value. The value is determined by how quickly, if at all, a pet is adopted. The values are determined in the following way:
0 - Pet was adopted on the same day as it was listed.
1 - Pet was adopted between 1 and 7 days (1st week) after being listed.
2 - Pet was adopted between 8 and 30 days (1st month) after being listed.
3 - Pet was adopted between 31 and 90 days (2nd & 3rd month) after being listed.
4 - No adoption after 100 days of being listed. (There are no pets in this dataset that waited between 90 and 100 days).

Submissions are scored based on the quadratic weighted kappa, which measures the agreement between two ratings

Data Preprocessing and Modelling : The sentiment, metadata and rating was extracted from JSON file. Feature Engineering was created, Text was converted into vector using TD-IDF, information was extracted from image files. Modelling was performed using LGB algorithm and result was evaluated on quadratic weighted kappa
