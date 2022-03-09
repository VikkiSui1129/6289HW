a. 
![alt text](https://github.com/VikkiSui1129/6289HW/blob/f36f56561cade9af0d7a26fc7fdd93437aeeb4a9/HW2/q1.png)
As the number of hidden layers increases, there is a shape increase from 0 to 1 hidden layer, but there is no big improvement from 1 hidden layer to 4 hidden layers. This is because adding the first hidden layer will increase the number of parameter a lot, but that size of parameter is probably enough for the model, so adding more hidden layers did not improve the test accuracy. Besides, the convolutional neural network has the highest accuracy. The 2D convolution can learn local information from neighbor pixels. It can catch more 2D information while the dense layers can only learn 1D information.

b. 
![alt text](https://github.com/VikkiSui1129/6289HW/blob/f36f56561cade9af0d7a26fc7fdd93437aeeb4a9/HW2/q2.png)
When changing all Relu to Sigmoid, the network performs worse. Although at the beginning the network always give the random output (10% accuracy), after enough epochs, the network will perform better than current test accuracy.
Compared with the sigmoid, ReLU has a huge acceleration effect on the convergence of stochastic gradient descent. Sigmoid contains exponential operations during derivation, while ReLU derivation has almost no computation.

c. 
![alt text](https://github.com/VikkiSui1129/6289HW/blob/f36f56561cade9af0d7a26fc7fdd93437aeeb4a9/HW2/q3_1.png)
![alt text](https://github.com/VikkiSui1129/6289HW/blob/f36f56561cade9af0d7a26fc7fdd93437aeeb4a9/HW2/q3_2.png)
1. The training accuracy always keep increasing. CNN without dropout or data augmentation has the highest training accuracy. This model is overfitted.
2. 2. A lightweighted CNN network can't hold all information from a large dataset. If the model capacity is already low, lowering it further by adding dropout will hurt performance. As you can see the training/test accuracy becomes lower.
3. 3. Data augmentation (horizontal/vertical flip) will reduce the overfitting problem. It will make the training accuracy and test accuracy closer. And test accuracy won't decrease even when training for large epochs.
