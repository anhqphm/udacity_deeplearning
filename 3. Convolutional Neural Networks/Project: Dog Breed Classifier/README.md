This is a project done for Udacity Deep Learning.

Things to further deep dive:

1) Try going deeper and wider i.e try going deeper by using more layers and wider by using more filters. You have just gone 3 convs deep and 128 filters wide. Try something like a Resnet 50 with 1024 filters which  you have also used for transfer learning . Generally a depth/width ratio also becomes a hyperparameter. Like Resnet 152 is good but one thing you will learn is that how fast will such a network be during test time i.e when used in real time on an embedded system?

2) One thing that I recently learnt and I haven't seen many people working on it is that after having trained your network using SGD and achieving local minima, try using ADAM on the learnt weights and try reaching a global minima.

3) I think you should have used more epochs as the losses were constantly going down and you would have achieved better accuracy for the CNN you built from scratch. I understand 100 epochs were a good enough number of training and meeting the requirement but it would have been interesting to see when does the model start to overfit. Moreover, for learning, you can try different type of convolutions and see what output you get. For example depth wise separable convs, spatial and cross channel convs. For a very basic idea, check this article https://ikhlestov.github.io/pages/machine-learning/convolutions-types/

You can also check this article for a deeper understanding -> https://www.analyticsvidhya.com/blog/2018/12/guide-convolutional-neural-network-cnn/

Your answer about the improvements is quite interesting. You can also use batch normalization and read about the same here - https://arxiv.org/pdf/1502.03167.pdf. Though there have been many debates and research about batch norm but I still feel that this paper forms the foundation for understanding further debates about batch norm.
