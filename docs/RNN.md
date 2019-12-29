we've been looking at convolutional neural networks and models that allows us to analyze the spatial information in a given input image. CNN's excel in tasks that rely on finding spatial and visible patterns in training data.These networks give us a way to incorporate memory into our neural networks, and will be critical in analyzing sequential data. RNN's are most often associated with text processing and text generation because of the way sentences are structured as a sequence of words, but they are also useful in a number of computer vision applications, as well!

https://video.udacity-data.com/topher/2018/May/5af0e03b_video-classification/video-classification.pdf

RNNs have a key flaw, as capturing relationships that span more than 8 or 10 steps back is practically impossible. This flaw stems from the "vanishing gradient" problem in which the contribution of information decays geometrically over time.

What does this mean?

As you may recall, while training our network we use backpropagation. In the backpropagation process we adjust our weight matrices with the use of a gradient. In the process, gradients are calculated by continuous multiplications of derivatives. The value of these derivatives may be so small, that these continuous multiplications may cause the gradient to practically "vanish".

LSTM is one option to overcome the Vanishing Gradient problem in RNNs.

Please use these resources if you would like to read more about the Vanishing Gradient problem or understand further the concept of a Geometric Series and how its values may exponentially decrease.



## Why do we need RNNS?
* RNNs are used for time series analysis.
* When you need to make a prediction based on previous data, not only the current data. They make use of sequential information.
* Example :
  **Stock Price Prediction**.
  **Text Generation**

**A RNN is multiple copy of the same network that receives the inputs at different times as well as it's previous hidden state**.

<img src="https://upload.wikimedia.org/wikipedia/commons/b/b5/Recurrent_neural_network_unfold.svg" alt="hi" class="inline"/>
