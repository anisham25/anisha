---
_archived: false
_draft: false
created-on: "2021-08-24T21:40:11.247Z"
name: "Quantum Machine Learning Is The Next Big Thing."
slug: "quantum-machine-learning-is-the-next-big-thing"
subheader: "Utilizing machine learning algorithms on quantum computers to unlock a new era of problem solving"
date: "2020-05-20T00:00:00.000Z"
updated-on: "2021-08-25T02:12:16.602Z"
published-on: "2021-08-25T02:14:02.520Z"
tags: "post"
layout: "single-post.html"
---

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e540d09ec577b3b72d7_0*XcIix2xbLzNEIXAH.png)

Most of us have heard of AI and quantum computing. But, have we heard of **quantum machine learning**?

Quantum machine learning is the intersection between quantum computing and AI that’s going to change what the future looks like.

Individually, they’re amazing. But together, they’re unstoppable.

Quantum machine learning is **a field that aims to write quantum algorithms to perform machine learning tasks.**

In this article, I’m going to break down those intimidating words. Specifically, I’m going to be talking about quantum support vector machines (QSVMs) but there tons of other QML algorithms to learn about.

Classical Machine Learning
--------------------------

Machine learning can be broken down into three core groups: **supervised** **learning**(training data to predict the next value), **unsupervised** (acting on unlabeled data), and **reinforcement** (learning from environment and mistakes).

Support vector machines (SVMs) fall into the category of supervised learning and we’re going to be focusing on that.

**Supervised learning algorithms learn from examples.** In supervised learning, you have input variables (X) and an output variable (Y). The purpose of the algorithm is to learn how the function maps from the input to the output.

Y = f(X)

The algorithm’s goal is to approximate the mapping function well enough that when you have new input data (X), you can predict the output variables (Y) for that data.

For example, the supervised learning algorithm can use a trained dataset to understand the difference between two types of objects (cats and dogs). The algorithm analyzes the different features (hair, color, eyes, ears, etc.) to learn what each object looks like. Then, an unknown data point is introduced (a white dog). Using its past training, the algorithm will predict which category the data point falls into.

It is called supervised learning because it’s similar to a teacher giving information to a student. The teacher gives out the answer at first for the student (or in this case the algorithm) to learn. But, eventually, the student understands the concepts enough to solve problems on their own.

Support Vector Machines
-----------------------

SVMs are among the most powerful supervised learning algorithms. In this case, we use them for classification but they can also be used for regression.

Their specialty comes from their ability to **classify objects in the nth-dimensional space** (N–the number of features).  Their objective is to find a hyperplane in nth-dimensional space that distinctly classifies the data points.

To understand, it helps to think of an analogy. Picture drawing a cat and putting a dog sticker right on top of the cat drawing. It’s 2D (n=2); regardless of how many lines you draw, there’s absolutely no way to separate the cat and dog. The two dimensions (i.e. weight and height) aren’t enough to classify the object.

This is the problem that many classification algorithms deal with.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e54bae02802ee52ca4d_0*QtqSrSmbJtXiNp2l.png)

2D hyperplane

Now, let’s make it 3D(n=3) by adding another dimension; depth. We realize that the two objects are eclipsed, inhabiting different depths. The third dimension (i.e. bark) allows the computer to understand the difference. If we project the cat and dog into a higher-dimensional space, we can slide a thin sheet (a “plane”) between the two to separate them.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e54a070c615dddf885c_0*n6iH0uqfIp7U-q-L.png)

3D hyperplane

Although it’s very simple, this is what SVMs do. They analyze in the **nth dimensional space.**

The computers take the images of a cat or dog and organize their pixels based upon height, weight, bark, and other characteristics. Then, the computer utilizes a **kernel trick** to project the non-linear data set into a higher dimensional space. The end result is the **“feature map”** which allows us to understand how input (X) becomes output (Y).

But’s what’s the holdup with classical machine learning and SVMs? Why do we even need to add quantum computers?

Quantum Machine Learning
------------------------

When data points are projected in higher and higher dimensions, it is hard for classical computers to deal with such large computations. Even if the classical computer can handle it, it would take too much time.

Simply put, **sometimes, classical machine learning algorithms are too taxing for classical computers.**

Luckily, quantum computers have the computational power to handle these taxing algorithms. They utilize powerful laws like superposition and entanglement to solve problems faster than their classical counterparts.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e54254034134521bf1a_0*St4Q17pUxJKDd022.png)

In fact, [a study by IBM and MIT](https://www.nature.com/articles/s41586-019-0980-2) found that SVMs are, mathematically, very similar to what goes on inside a quantum computer.

Using quantum machine learning, scientists can turn a classical machine learning algorithm into a quantum circuit so it can be run efficiently on a quantum computer.

Applications
------------

Quantum machine learning is an extremely new field with so much more growth. But, we can already start to predict how it’s going to impact our future!

Here are some of the areas QML will disrupt:

*   Understanding nanoparticles
*   The creation of new materials through molecular and atomic maps
*   Discovering new drugs and medical research
*   Understanding the deeper makeup of the human body
*   Enhanced pattern recognition and classification
*   Furthering space exploration
*   Creating complete connected security through merging with IoT and blockchain

With more amazing developments happening every day, QML will solve more problems in the coming decades than we could’ve ever imagined.

Personal Project: Utilizing SVMs for Classification of Parkinson’s Disease
--------------------------------------------------------------------------

I built a QML algorithm to identify whether a patient has Parkinson’s disease based on their speech features. I conducted a 9-qubit simulation on IBM’s quantum simulators utilizing a quantum support vector machine.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e5496de656ca9c98695_0*JAkDgIEDZHGwCZbD.png)

**How to build the algorithm:**
-------------------------------

The first step is to set up the circuit:

1.  Import the necessary packages
2.  Load your IBM account credentials and connect to the optimal quantum simulator
3.  Set up the number of shots (or attempts) your algorithm will take

The next step is to prepare the dataset:

1.  Import the dataset. The Parkinson’s dataset I used can be found [here](https://archive.ics.uci.edu/ml/datasets/Parkinson%27s+Disease+Classification#).
2.  Split the data into the two classes (present and not-present)
3.  Divide the data into training and testing datasets (a 7:3 training to testing ratio is ideal)

Then, we need to build the QML algorithm:

1.  Set up the number of qubits the circuit will have (the number of qubits should be equivalent to the number of features in your dataset)
2.  Initialize the feature map to build the SVM
3.  Set the necessary parameters; including the device it’ll run on, number of shots, and initializing the pseudo-random number generator
4.  Import unlabelled data for classification

The last step is to run the algorithm. The run method will generate the accuracy of the circuit. Meanwhile, the predict method will do the training, testing, and prediction of the unlabeled data.

![Image for post](https://uploads-ssl.webflow.com/61241da8381f9c35320e4962/61255e542219ee3967e2adff_1*vfbOnzADo2LUJZ4M40SciA.png)

Results of the QSVM

The results shown can predict whether or not each of 9 patients have Parkinson’s disease with a 0.75 accuracy rate. With a larger dataset and more stable hardware, the accuracy rate will only go up.

Future Implication
------------------

With diseases like Parkinson’s, the earlier the detection, the better the treatment. QML algorithms like this one will be able to make huge strides in treatment and disease prevention.

In the coming years, quantum machine learning is going to become a massive field with increasingly more computational power. It’ll have the capability to solve the world’s most complex problems. The AI revolution of today will be even bigger when combined with quantum computing.

I’m super excited to see the field grow and become integrated into our lives. Lucky for us, many QML experiments are already possible with our current quantum technology. QML is already here and we’re ready for it!

**Github for reference to the project:** [https://github.com/anisham25/parkinsons-QSVM](https://github.com/anisham25/parkinsons-QSVM)

‍

‍

**Personal Website:** [www.anishamusti.com](http://www.anishamusti.com/)

_My name is Anisha Musti. I’m 15 years old and passionate about quantum computing and artificial intelligence. Thank you for reading and I hope you learned something! Stay up to date for more articles on quantum computing, AI, and other interesting technologies._

Connect with me on LinkedIn [here](https://www.linkedin.com/in/anisha-musti-056703180/) and email me at anisha.musti@gmail.com for any inquiries.
