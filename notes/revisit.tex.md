## Lesson 2

Why is there a sum in the [following](https://classroom.udacity.com/nanodegrees/nd101/parts/94643112-2cab-46f8-a5be-1b6e4fa7a211/modules/89a1ec1d-4c22-4a77-b230-b0da99240c89/lessons/07f472eb-0210-446f-8ec2-d297b06c86d0/concepts/87d85ff2-db15-438b-9be8-d097ea917f1e):

> To update the weights to hidden layers using gradient descent, you need to know how much error each of the hidden units contributed to the final output. Since the output of a layer is determined by the weights between layers, the error resulting from units is scaled by the weights going forward through the network. Since we know the error at the output, we can use the weights to work backwards to hidden layers.

> For example, in the output layer, you have errors $\delta^o_k$ attributed to each output unit $k$. Then, the error attributed to hidden unit $j$ is the output errors, scaled by the weights between the output and hidden layers (and the gradient):

> ![revisit01.gif](revisit01.gif)

I pretty sure that this should be a sum over $k$, the output units.

Search for Lesson 2 notes implementation line:

```hidden_error = np.dot(output_error_term, weights_hidden_output)```

Further learning:

* [Karpathy: Yes you should understand backprop](https://medium.com/@karpathy/yes-you-should-understand-backprop-e2f06eab496b)
* [Karpathy: Backprop from CS231n](https://www.youtube.com/watch?v=59Hbtz7XgjM)

