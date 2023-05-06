Download Link: https://assignmentchef.com/product/solved-ece495-midterm
<br>
<h2>Q1. ADS Fundamentals</h2>

1a. A vehicle is equipped with a stop-and-go pilot, which can fully operate a vehicle on a highway in traffic jams, but with a fallback-ready user. Which level(s) of driving automation is this driving automation system operating at?

<h2>Q2. Computer Vision Fundamentals</h2>

2a. Compute 1-D cross-correlation by applying the following filter [0 2 1] to the following signal [0 1 3 0] (assume enough zero padding to show all non-zero output)




2b. Assume that the output of cross-correlating the 1-D filter [2 3 2] with some input signal resulted in the following output signal [7 10 7]. What would be the output signal have we used convolution instead of cross-correlation and why?

The result of cross-correlation and convulsion in this instance are the same with this specific filter. This is because during convolution the filter is “flipped”, but in this instance the filter is symmetric.

1

2d. What is the name of the following filter and what is it computing?




.

2f. Why is the Canny filter using double thresholding? [1 mark]

2g. Consider the following representation in Hough space (polar coordinates).

<table width="601">

 <tbody>

  <tr>

   <td width="601">2h. Which of the following value profiles represent black in HSV? (select all that apply) [1 mark]1.    0,high,high2.    any,low,low3.    any,low,high4.    60,high,high5.    any,high,low6.    any,any,low</td>

  </tr>

 </tbody>

</table>

<h2>Q3. Machine Learning Fundamentals</h2>

3a. Starting with the probabilistic model for linear regression (assume single input <em>x </em>and single out <em>y</em>), show that maximizing the likelihood for a dataset (<em>x</em>, <em>y</em>) (with i.i.d. datapoints) is equivalent to minimizing the sum of squared errors. Hint: go via negative log likelihood [5 marks]

(3)

<em>i</em>=1

3b. What is the regression loss (as used in class) for a data point with label 0.4 and predicted output 0.7? [1 mark]

(4)

3c. (Apply what you’ve learned in lecture and Assignment 2) Given the following set of input vector <em>X</em>, ground truth vector <em>Y</em>, and weight matrices <em>W</em><sub>1</sub>, <em>W</em><sub>2</sub>, <em>B</em><sub>1</sub>, and <em>B</em><sub>2 </sub>of a 2 layer fully connected neural network, what is the inference probability of the correct class? What is the cross-entropy loss value? Assume ReLU activation on the first hidden layer and softmax activation on the output layer. Show each step of the computation. Hint: Use numerically stable softmax and assume <em>e</em><sup>−1 </sup>≈ 0.37 and <em>e</em><sup>−7 </sup>≈ 0.00 [5 marks]




<table width="601">

 <tbody>

  <tr>

   <td width="601">3d. Consider the computational graph below for the following function<em>f</em>(<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>) = <em>ln</em>(3<em>x</em><sub>1 </sub>+ <em>e</em><sup>2<em>x</em></sup><sup>2</sup>)                                                   (8)Draw the computational graph and annotate it with the forward pass (above the arrows) and backward pass (below the arrows) for <em>x</em><sub>1 </sub>= 1 and <em>x</em><sub>2 </sub>= 0 (propagate the gradient back to each function input). Recall<em>de</em><em>x </em>= <em>e</em><em>x                  </em>(9) <em>dx</em><em>dln</em>(<em>x</em>)       1=     (10) <em>dx x</em>Assume <em>ln</em>(4) ≈ 1.39 [5 marks]</td>

  </tr>

 </tbody>

</table>




3e. What is the difference between Stochastic Gradient Descent and ordinary (Batch) Gradient Descent? [

.

3f. How is the condition of overfitting defined?

3g. Consider a convolutional layer with an input volume of depth 4 and output volume of depth 128. How many convolutional filters does the layer contain? What is the depth of each filter? [

<h2>Q4. Semantic Segmentation</h2>

4a. (Apply what you’ve learned in lecture and Assignment 3) Semantic segmentation architectures sometimes use skip connections from early feature maps of the feature extractor to the corresponding-size upsampled maps in the decoder. What is the role of these connections? [1 mark]

4b. (Assignment 3) You were recommended to use batch norm as part of your network. Given a layer with the linear transformation and an activation function, where is the batch norm operation normally applied?

<h2>Q5. Object Detection</h2>

5a. Assume that an object detector uses a 5-by-5 grid and 3 anchor boxes at each cell. What is the maximum number of objects that the detector can detect? [1 mark]

.

5b. On a test set with a total of 4 of cars in the ground truth, a detector produced 3 bounding boxes with the following (score, IoU): (0.5,0.7), (0.7,0.8), (0.9, 0.2) (assume that each returned bounding box overlaps with a different ground truth). Assuming a score threshold of 0.6 and IoU threshold of 0.6, specify the number of TP, FP, and FN. [3 marks]

5d. How is it possible for two different bounding boxes to be generated for the same object (before non-maximum suppression)? [1mark]




<table width="601">

 <tbody>

  <tr>

   <td width="601">5e. Which of the statements is correct?a)    An output neuron in an object detector is influenced only by input pixels withinthe anchor box assigned to it.b)    An output neuron in an object detector is influenced only by input pixels withinits positive anchor box.c)     An output neuron in an object detector is influenced only by input pixels withinits empirical receptive field.</td>

  </tr>

 </tbody>

</table>