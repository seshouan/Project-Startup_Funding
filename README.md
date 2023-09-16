# Project-Startup_Funding
A binary classification model using a deep neural network to predict whether funding applicants will be successful

#### Code Source: venture_funding_with_deep_learning.ipynb

## Results of analysis

### Original model:

=================================================================<br>
 dense_15 (Dense)            (None, 16)                1872      
                                                                 
 dense_16 (Dense)            (None, 8)                 136       
                                                                 
 dense_17 (Dense)            (None, 1)                 9         
                                                                 
=================================================================<br>
Total params: 2017 (7.88 KB)
Trainable params: 2017 (7.88 KB)
Non-trainable params: 0 (0.00 Byte)

Original Model Results
268/268 - 0s - loss: 0.5656 - accuracy: 0.7224 - 319ms/epoch - 1ms/step
Loss: 0.5655603408813477, Accuracy: 0.722449004650116

### Alternative 1: ###

=================================================================<br>
 dense_18 (Dense)            (None, 32)                3744      
                                                                 
 dense_19 (Dense)            (None, 16)                528       
                                                                 
 dense_20 (Dense)            (None, 1)                 17        
                                                                 
=================================================================<br>
Total params: 4289 (16.75 KB)
Trainable params: 4289 (16.75 KB)
Non-trainable params: 0 (0.00 Byte)

Alternative Model 1 Results
268/268 - 0s - loss: 0.5673 - accuracy: 0.7233 - 381ms/epoch - 1ms/step
Loss: 0.5672855377197266, Accuracy: 0.7232652902603149

### Alternative 2:

=================================================================<br>
 dense_21 (Dense)            (None, 64)                7488      
                                                                 
 dense_22 (Dense)            (None, 32)                2080      
                                                                 
 dense_23 (Dense)            (None, 16)                528       
                                                                 
 dense_24 (Dense)            (None, 16)                272       
                                                                 
 dense_25 (Dense)            (None, 1)                 17        
                                                                 
=================================================================<br>
Total params: 10385 (40.57 KB)
Trainable params: 10385 (40.57 KB)
Non-trainable params: 0 (0.00 Byte)

Alternative Model 2 Results
268/268 - 0s - loss: 0.5761 - accuracy: 0.7213 - 402ms/epoch - 1ms/step
Loss: 0.5761035680770874, Accuracy: 0.7212827801704407

## Conclusion

While adding more nodes to the 2 hidden layers achieved a slightly better accuracty, increasing the number of layers to 4 actually decreased the accuracy.

We would need to tweak more variables to improve the overal accuracy of the model, as it is presently quite low.
