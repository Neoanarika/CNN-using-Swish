# CNN using swish 

Swish was introduce on oct 2017 as an alternative
activation function to relu. Swish was found using a combinaton exhaustive 
search and reinforcement learning. In the originial paper [1], swish was 
demostrated improvement of top-1 classification by ImageNet by 0.9% by simply
replacing all relu activation functions with swish. Nonethless, swish is 
very easy to implement just writing 1 line of code is enough to implement swish 
in tensorflow

## Example

```
x1 = tf.nn.conv2d(X, W1, strides=[1,1,1,1], padding='SAME') + B1
Y1 = x1*tf.nn.sigmoid(x1)# output is 28x28
```

# Results 

![alt text](https://github.com/Neoanarika/CNN-using-Swish/blob/master/media/loss_swish.png)

During the inital phase of training the loss function remains , on average, the same this shows that swish suffers from poor intialisation during training, at least when using initally normal distributed weights with std_dev =0.1. 

# Reference 
1. Searching for Activation Functions https://arxiv.org/abs/1710.05941
