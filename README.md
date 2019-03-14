# Species_Classification
Attempt to use CNN to classify three species.
A sparse data set of only 422 images were taken.
Images were sorted and placed in train test and validation folders.
Each folders contains 3 sub folders Species A, SpeciesB and SpeciesC.
Keras was used the classification category flowed from the directory.
**In the first attempt a very low val_accuracy of 33% was obtained**.
**In the second attempt a reasonable val_accuracy of 58 and a highest of 75% was obtained.**\n
**The model was tuned to get a stable result and ended out to have a val_accuracy somwhere near 60%**. 

Further improvement and paramter tuning are still going on.
Please Note: The training was done in a CPU without using GPU so there is a very high chance of getting better accuracy with GPU.
The data set is hosted in Sciebo and if anyone insterested can contact me.\n
## Model Evaluations
In the first model there were less fluctuations in the validation set and had a poor accuracy of 35% the batch size was about 20 but and the pictures were normalised into a tensor took a lot of time to train for 10 epochs may have had better results with more epochs.

In the second model the pictures were normalised but the batch sizes were decreased it made high accuracy of 75% but was as random as flipping a coin. As the acuraccies fluctuated very much it was of no use.

In the third model the batch siye for both the training and testing set was inreased so as was the learning rate of the optimiser this gave us a stable increase in val_accuracy and gave a near about 60%. Training a model from scratch and with a sparse dataset for me this was really fulfilling!
