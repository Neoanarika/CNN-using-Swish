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
Y1 = x1*tf.nn.sigmoid(beta1*x1)# output is 28x28
```

# Reference 
1. Searching for Activation Functions https://arxiv.org/abs/1710.05941
