# Exploring-GMMs-CNNs-and-Sequence-Algorithms
In this notebook I derive mathematical equations for GMMs, CNNs, Prefix Span, and Sequence Alignment. I also coded a Gaussian Mixture Model from scrath, implemented the Apriori Algorithm, and constructed a convolutional neural network. 

## Derviations

- **EM Derivations for a Gaussian Mixture Model (GMM)**
  Dervied the proof for the maximum liklihood estimates for a GMM with soft assignments, starting from the complete-data log liklihood expression

- **Calculated One Convolution (CNN)**
  Using a given input image and filter, I calculated the result of the valid convolutional result after passing the filter over the image using matrix multiplication, indicating each of my intermediary calculations.

- **Prefix Span Calculation**
  Given an example dataset, I found the freqent single-item sequences, derived the projected database for one frequent item, and used that projected database to find all possible 2-item extensions of that prefix that are still frequent.

- **Sequence Alignment**
  Given two DNA sequences, I constructed the DP Table, backtracked using the Bellman-Ford algorithm to find the optimal alignment of the two sequences and calculated the optimal alignment score.

## Coding
- **Gaussian Mixture Model**
  I loaded the example dataset from sklearn, conducted data preprocessing, trained a GMM from sklearn, and experiemented with a variety of component numbers and covariance types to find the combination that captured trends in the dataset most optimally (lead to the most optimal cluster assigments of the data). I then visualized the data, including cluster assingments and the planes separating clusters to visualize how well-separated the clusters were.

- **Implementing the Apriori Algorithm**
  I loaded the dtaset and implemented the Apriori algorithm, generating 1-itemsets, counting their frequencies and generating k-itemsets for valid candidates, pruning candidates using the Apriori property. I continued this process until there were no more frequent itemsets remaining. I experiemented with different values for the minimum support threshold and generated association rules, along with their metrics (confidence and lift).


- **Convolutional Nerual Network (CNN)**
  Using PyTorch, I build a simple CNN trained on the CIFAR-10 dataset. I experiemented with model architecture and tuned the model, varying the number of hidden layers/max pooling layers, kernel size, and the learning rate. I used the Adam optimizer, ReLU activation function, and the cross entropy loss function. 
