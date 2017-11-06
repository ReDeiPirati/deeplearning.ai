# Coursera deeplearning.ai - Deep Learning Specialization - Improving Deep Neural Networks: Hyperparameter tuning, Regularization and Optimization

This document contains a guide to help you to start experimenting with [Coursera deeplearning.ai](https://www.coursera.org/specializations/deep-learning) specialization assignments **as easily as possible** through a Jupyter notebook running on [FloydHub](https://www.floydhub.com/).

The code in this project was ported from the [official course](https://www.coursera.org/learn/deep-neural-network), but only the necessary files to run this specific project were selected. The data used in this project is already available as a FloydHub dataset.

You can find the video lectures about Improving Deep Neural Networks  specialization on [Deeplearning.ai's official youtube channel](https://www.youtube.com/watch?v=1waHlpKiNyY&list=PLkDaE6sCZn6Hn0vK8co82zjQtt3T2Nkqc).

## Assignment 5: Tensorflow.

Welcome to the Tensorflow Tutorial! In this notebook you will learn all the basics of Tensorflow. You will implement useful functions and draw the parallel with what you did using Numpy. You will understand what Tensors and operations are, as well as how to execute them in a computation graph.

After completing this assignment you will also be able to implement your own deep learning models using Tensorflow. In fact, using our brand new SIGNS dataset, you will build a deep neural network model to recognize numbers from 0 to 5 in sign language with a pretty impressive accuracy.

## Run on FloydHub

Follow the next steps to get a jupyter notebook up and running for Assignment 5.

### 1. Create a FloydHub account

- [Sign up](https://www.floydhub.com/signup) on FloydHub
- Install the floyd CLI on your local machine through these two [steps](https://www.floydhub.com/welcome):

```bash
$ pip install -U floyd-cli

$ floyd login
# Follow the instructions on your CLI
```

### 2. Clone this project to your local machine

```bash
$ cd /path/to/your-project-dir
$ floyd clone udacity/projects/first-neural-network/8
```

### 3. Create your project version on FloydHub

[Create a project](https://www.floydhub.com/projects/create) on FloydHub and then sync the cloned repository with your new project:

```bash
$ floyd init your-project-name
```

### 4. Run the project through a jupyter notebook

- The `--mode` flag specifies that this job should provide us a Jupyter notebook.
- The `--data` flag specifies that the version 2 of the cat-vs-noncat dataset should be available at the `/datasets` directory
- The `--env` flag specifies the environment that this project should run on, which is a Tensorflow 1.1.0 + Keras 2.0.6 backend environment with Python 3.5.

```bash
floyd run \
    --mode jupyter \
    --env tensorflow-1.1 \
    --data redeipirati/datasets/cat-vs-noncat/4:datasets
```

Once the job is started, the jupyter notebook will open in your browser and you are ready to go!

## More about FloydHub platform

- Note that changes you make to the notebook running on Floyd servers are not going to be saved at your local directory, but they are going to be available in the [output](https://www.floydhub.com/udacity/projects/first-neural-network/8/output) section of your job.
- Once you stop the Jupyter notebook job you were running, from the job page, you can click on [Restart](http://blog.floydhub.com/restart-jupyter-notebook-workflow/?utm_medium=email&utm_source=21sep17) to restart your job exactly how you left it and optionally choosing another environment (CPU or GPU). This is a great way to spend less of your GPU hours if you are working on tasks that does not require a GPU.
- If you need any help check our [documentation](http://docs.floydhub.com/) and [forum](https://forum.floydhub.com/).

