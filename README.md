# Learning Deep Learning with TensorFlow

This is a compiled and revised repository of my teaching material for a course on deep learning with TensorFlow in 2021/22 and 2022/23 and is meant as a self-contained resource for self-study. 

Sessions 14 and 15 as well as exercises for the sessions are not yet available in this repository. They will be added when I find time to add content that is suitable for self-study.

How to study:
Go through the material sequentially, first reading/going through the session's notebook, supplementary material and possibly read some background reading, then do the exercise designated to that session (see table below).

Course contents:

|     Session     |    Content                             |              Exercise                 | Supplementary material |     Recommended or seminal readings |
|-----------------|----------------------------------------|---------------------------------------|------------------------|------------------------------------|
|   [00](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/00.ipynb)            |    Basic tensor operations in TensorFlow + Prerequisites|               [Exercise0](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise0.ipynb)               |    -   |   [Mathematics for Machine Learning book](https://mml-book.github.io/book/mml-book.pdf)|
|   [01](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/01.ipynb)            |    From biological neurons to logic gates, to activation functions to universal function approximation (build your first ANN from scratch)                            |                 [Exercise01](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise01.ipynb)                      |  [deriving matrix multiplication gradients 1](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/02_matmul_derivative_1.pdf), [deriving matrix multiplication gradients 2](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/02_matmul_derivative_2.pdf)  | [McCulloch & Pitts (1943)](https://link.springer.com/article/10.1007/bf02478259) |
|   [02](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/02.ipynb)            |   Learning in ANNs: Gradient Descent, Backpropagation, and Automatic Differentiation (build your first ANN from scratch, including backpropagation and training loop)                                |                [Exercise02](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise02.ipynb)                       | - |  [Rumelhart, Hinton & Williams (1986)](https://apps.dtic.mil/dtic/tr/fulltext/u2/a164453.pdf) |
|   [03](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/03.ipynb)            |       Basic usage of TensorFlow's automatic differentiation: The GradientTape context manager                      |            -                           | - |  [TensorFlow's autodiff guide](https://www.tensorflow.org/guide/autodiff), [TensorFlow's advanced autodiff guide](https://www.tensorflow.org/guide/advanced_autodiff) |
|   [04](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/04.ipynb)            |       Modules, Layers, and Models. An introduction to the Keras Subclassing API                |  -  | -  | [TensorFlow's intro to modules](https://www.tensorflow.org/guide/intro_to_modules) |
|    [05](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/05.ipynb)            |    Keras metrics for keeping track of losses, accuracies etc.              |     -          |   -   | - |
|    [06](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/06.ipynb)            |      Loss functions and optimizers           |       [Exercise03](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise03.ipynb)        |  -  | [Kingma & Ba (2015)](https://arxiv.org/abs/1412.6980), [Bishop (2006), chapters 3+4](https://github.com/peteflorence/MachineLearning6.867/blob/master/Bishop/Bishop%20-%20Pattern%20Recognition%20and%20Machine%20Learning.pdf) |
|    [07](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/07.ipynb)            |      Putting it together: Using TensorBoard to log training data and implementing a subclassed model using keras metrics and a custom training loop.           |       -        |   -  | - |
|    [08](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/08.ipynb)            |     Convolutional Neural Networks (incl. interactive widget)           |       [Exercise04](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise04.ipynb)        |   -   | [Goodfellow, Bengio & Courville (2016), chapter 9](https://www.deeplearningbook.org/contents/convnets.html), [Krizhevsky, Sutskever & Hinton (2012)](https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf), [Simonyan & Zisserman (2014)](https://arxiv.org/abs/1409.1556), [He, Zhang, Ren et al. (2015)](https://arxiv.org/abs/1512.03385), [Huang, Liu, van der Maaten et al. (2017)](https://arxiv.org/abs/1608.06993) |
|    [09](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/09.ipynb)            |     Regularization: Avoiding overfitting with L1/L2 penalties, dropout, normalization and data augmentation           |       [Exercise05](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise05.ipynb)        |    -     | [Goodfellow, Bengio & Courville (2016), chapter 9](https://www.deeplearningbook.org/contents/regularization.html), [Srivastava, Hinton, Krizhevsky et al. (2014)](https://www.cs.toronto.edu/~hinton/absps/JMLRdropout.pdf), [Bishop (2006), chapter 5.5](https://github.com/peteflorence/MachineLearning6.867/blob/master/Bishop/Bishop%20-%20Pattern%20Recognition%20and%20Machine%20Learning.pdf)|
|    [10](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/10.ipynb)            |     Optimization difficulties: Vanishing and exploding gradients. Weight initialization, normalization and residual/skip connections as partial solutions           |       [Exercise06](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/Exercise06.ipynb)        |    -     | [He, Zhang, Ren et al. (2015)](https://arxiv.org/abs/1512.03385), [Ba, Kiros & Hinton (2016)](https://arxiv.org/abs/1607.06450), [Goodfellow, Bengio & Courville (2016), chapter 8](https://www.deeplearningbook.org/contents/optimization.html)  |
|    [11](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/11.ipynb)            |     Recurrent Neural Networks: From unrolled recurrence to dynamically unrolled custom recurrent cells           |       Exercise07        |     -     | [Hochreiter & Schmidhuber (1997)](https://www.bioinf.jku.at/publications/older/2604.pdf), [Cho, van Merrienboer & Gulcehre (2014)](https://arxiv.org/abs/1406.1078v3), [Elman (1990)](https://doi.org/10.1016/0364-0213(90)90002-E), [Sherstinsky (2020)](https://sci-hub.se/10.1016/j.physd.2019.132306)|
|    [12](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/12.ipynb)            |     Autoencoder           |       Exercise08        |     -     | - |
|    [13](https://github.com/Spinkk/Teaching-TensorFlow/blob/main/13.ipynb)            |     Generative Models           |       Exercise09        |    -      | - |
|    (14)            |     Transformers and NLP           |       Exercise10        |    -       | - |
|    (15)            |     Deep Reinforcement Learning           |       Exercise11        |   -     | - |
