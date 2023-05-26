# Thermotolerance-Gene-Prediction
Predicting genes involved in heat resistance in Candida auris

Files ending in .gz are the tokenised data files used for training, validation and testing.
The .csv files are the model’s predicted labels made using these input files, as well as a file containing the genes predicted as related to heat resistance (identified_heat_sequences.csv).

The config.json file is the configuration file necessary to run the trained model. The model itself could not be uploaded due to file size constraints but is available upon request. 

The code is split across tokensier.ipynb for tokenising the labelled data (model dataset), unannotated_tokeniser.ipynb for tokenising the unannotated C. auris sequences, and trainer.ipynb for training the model and making inferences. The trainer.ipynb notebook has several cells, which are each independent. The purpose of each is specified as an uppercase title at the top of the cell.

It should be noted that the metrics calculated during training are inaccurate due to a bug, and metrics were calculated separately using labels predicted by the trained model. The code for calculating metrics was retained for potential future development, but does not affect the model training.

The original datasets have not been included due to their file sizes, but are available upon request, or can be recreated and downloaded from https://fungidb.org/fungidb/app.

Filepaths are specific to the training system, and will need to be adjust to run any code.
