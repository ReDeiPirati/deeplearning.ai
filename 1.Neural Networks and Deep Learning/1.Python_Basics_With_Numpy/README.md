# Coursera deeplearning.ai - Deep Learning Specialization - Neural Networks and Deep Learning

This document contains a guide to help you to start experimenting with [Coursera deeplearning.ai](https://www.coursera.org/specializations/deep-learning) specialization assignments **as easily as possible** through a Jupyter notebook running on [FloydHub](https://www.floydhub.com/).

The code in this project was ported from the [official course](https://www.coursera.org/learn/neural-networks-deep-learning), but only the necessary files to run this specific project were selected. The data used in this project is already available as a FloydHub dataset.

You can find the video lectures about Neural Network and Deep Learning  specialization on [Deeplearning.ai's official youtube channel](https://www.youtube.com/watch?v=CS4cs9xVecg&list=PLkDaE6sCZn6Ec-XTbcX1uRg2_u4xOEky0).

## Assignment 1: Python Basics with Numpy

Welcome to your first programming exercise of the deep learning specialization. In this assignment you will:

- Learn how to use numpy.

- Implement some basic core deep learning functions such as the softmax, sigmoid, tanh, etc...

- Learn how to handle data by normalizing inputs and reshaping images.

- Recognize the importance of vectorization.

- Understand how python broadcasting works.

## Run on FloydHub

Follow the next steps to get a jupyter notebook up and running for Assignment 1.

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

- The `--mode` flag specifies that this job should provide us a Jupyter notebook
- Since its a basic tutorial on Python and Numpy you do not need to specify a certain environment because every FloydHub environments satisfy the depencies required.

```bash
floyd run \
    --mode jupyter
```

Once the job is started, the jupyter notebook will open in your browser and you are ready to go!

## More about FloydHub platform

- Note that changes you make to the notebook running on Floyd servers are not going to be saved at your local directory, but they are going to be available in the [output](https://www.floydhub.com/udacity/projects/first-neural-network/8/output) section of your job.
- Once you stop the Jupyter notebook job you were running, from the job page, you can click on [Restart](http://blog.floydhub.com/restart-jupyter-notebook-workflow/?utm_medium=email&utm_source=21sep17) to restart your job exactly how you left it and optionally choosing another environment (CPU or GPU). This is a great way to spend less of your GPU hours if you are working on tasks that does not require a GPU.
- If you need any help check our [documentation](http://docs.floydhub.com/) and [forum](https://forum.floydhub.com/).

