4th March 2019
==================

In this meeting, Ximing tried to share his idea of how convolutions work. Sharon also shared her questions and understanding during the meeting. Please check meeting videos for every detail.

###################
Minnor issue
###################

Please get involved more if possible.

###################
Conv Layer
###################

************************
What is Neural Network
************************

* Goal: to approximate some function :math:`f^*(x)`. 
* Example: A classifier such as `Digit Recognizer <https://www.kaggle.com/c/digit-recognizer>`_ . We are trying to map an input :math:`\boldsymbol{x}` to a category :math:`y`. As the example of Digit Recognizer, the input is an image of hand written digit. We are trying to approximate this function :math:`f^*(x)` with function f to map this image to the correct digit. 

************************
Convolution
************************

What is convolution in terms of vectors?

It is like applying a sliding window (we can call it kernel or filter) on top of the input of a layer. Example:

Our input is 

.. math::
	
	X = (x_1, x_2, x_3, .... , x_n)

Our Kenel (it contains all the parameters of the convolution) is 

.. math::

	K = (k_1, k_2, k_3)


The output of convolution is 

.. math::

	Y = 
	\begin {pmatrix}
		x_1k_1 + x_2k_2 + x_3k_3 \\
		x_2k_1 + x_3k_2 + x_4k_3 \\
		x_3k_1 + x_4k_2 + x_5k_3 \\
		...
	\end {pmatrix}

We are sliding the kernel on top of the input then apply the multiplication and sum to the corresponding input. Sliding would stop when the kenel reach the end of the input.

Sharon's question: how to integrate this image:

.. image:: rsc/NeuralNetwork.png

Ximing's understadning: This is an image for fully connected layer. Other then Convolution, we can also apply some other operation on the input of a layer. When you use matrix multiplication, the layer is called fully connected layer. There is no parameter sharing in 

In order to see how convolution is applied in matrix or tensor, please see the animation `here <http://cs231n.github.io/convolutional-networks/#conv>`_


############################
Suggestions
############################

* Get more prepared before the meeting. Trying to avoid draw diagram from scratch. 
* Putting tegother a slide would be much more helpful.


#########################
Resource shared this week
#########################

* `Sparse Autoencoder <https://www.youtube.com/watch?v=vfnxKO2rMq4&t=2848s>`_
* `A Comprehensive Guide to Ensemble Learning <https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-for-ensemble-models/>`_
* `Machine Learning with R and H2O <https://www.h2o.ai/wp-content/uploads/2018/01/RBooklet.pdf>`_
* `cs231n Convolutional Neural Networks  <http://cs231n.github.io/convolutional-networks/#conv>`_