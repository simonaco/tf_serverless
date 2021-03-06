Deploys a TensorFlow model to Azure Functions for hosting an Inferencing API.

Heavily relies on these instructions: https://docs.microsoft.com/azure/azure-functions/functions-create-first-function-python

## Forked from https://github.com/Vetal1977/tf_aws_lambda

This project is based on the above fork which deployed a TensorFlow model to AWS Lambda. This project shows how to do this on Azure Functions.

### Serverless serving of a TensorFlow model on Azure Functions
This is an extension of my [TensorFlow Serving test project](https://github.com/Vetal1977/tf_serving_example). It introduces a serverless serving of a sample GAN model, implemented with TensorFlow. It receives REST requests to predict [Street View House Numbers](http://ufldl.stanford.edu/housenumbers/).  
Mentioned GAN model is trained using [semi-supervised learning](https://en.wikipedia.org/wiki/Semi-supervised_learning) technique and based on the model taught at [Udacity Deep Learning Foundations](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101) course. The original Jupyter Notebook can be found at [GitHub](https://github.com/udacity/deep-learning/tree/master/semi-supervised).  
More details on the project can be found at my [blog](https://medium.com/@vitaly.bezgachev/serving-tensorflow-models-serverless-6a39614094ff).