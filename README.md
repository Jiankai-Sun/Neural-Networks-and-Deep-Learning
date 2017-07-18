# Neural-Networks-and-Deep-Learning
Code for Nielsen book "Neural Networks and Deep Learning". The online book can be find [here](http://neuralnetworksanddeeplearning.com/)

The [original code samples](https://github.com/mnielsen/neural-networks-and-deep-learning) is written for Python 2.6 or 2.7. Michal Daniel Dobrzanski has a repository for Python 3 [here](https://github.com/MichalDanielDobrzanski/DeepLearningPython35).

## Requirement:
Python >= 3.6.1  
IPython >= 6.0.0

## Note:
1. network2.py dosn't work currectly. Probably the reason is that training_data obtained from mnist_loader.py is a 'zip' object.

```python
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-1-c75e1cc25299> in <module>()
      4 net = network2.Network([784, 30, 10], cost = network2.CrossEntropyCost)
      5 net.large_weight_initializer()
----> 6 net.SGD(training_data[:1000], 400, 10, 0.5, evaluation_data=test_data, lmbda = 0.1, monitor_evaluation_cost=True, monitor_evaluation_accuracy=True, monitor_training_cost=True, monitor_training_accuracy=True)

TypeError: 'zip' object is not subscriptable
```

2. Untested    
  fig/more_data.py    
  fig/multiple_eta.py    
  fig/overfitting.py    
  fig/weight_initialization.py    

## Reference
[1] Michael A. Nielsen, "Neural Networks and Deep Learning", Determination Press, 2015 




