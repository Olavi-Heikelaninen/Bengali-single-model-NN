# Bengali-single-model-NN
https://www.kaggle.com/c/bengaliai-cv19
There're 2 main issues with the model:
1. It does not converge in 20 epochs, and even 20 is a bit too much given time constraint of 9h for CPU notebooks.
2. 1 is not obvious, need to add graphs to demonstrate.

One way to help with convergence is to set number of filters in conv_1 to 32, which, based on previous testing, shouldn't affect
performance too much, but will more than halve time per epoch.

Good thing is, its a pipeline from raw parquet data to submission file. No extra manipulations required.
