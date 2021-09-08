# DB Training Session

Tutorial on Natural Language Processing

### Date: September 9th from 8 to 9 am AEST


# Table of Contents

1. Libraries
2. The Data
3. Flash NLP Intro
4. Cleaning
5. Recommendation System
6. Topic Modeling (Optional)
7. Summary
9. Resources
10. Feedback 😃

Run this tutorial on Binder.  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ramonpzg/db_training/master)

Run this tutorial on Google Colab.  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SDjnvlfZBQ6VV985SeQkHBp6qRMKgPmE?authuser=1)


## Learning Outcomes

By the end of this tutorial you will

1. Have a better understanding of what is natural language processing and what are some of its applications.
2. Learn about the root of a word, what is means, and why we use them.
3. Be able to create a recommendation system based on text similarity.
4. Be able to conduct topic modeling on your own corpus.
5. Understand how to put together a simple app using panel.

Assumptions about you

- Have at least 1 year of coding experience in Python.
- Are comfortable with loops, functions, lists comprehensions, and if-else statements.
- Have some knowledge of pandas and NumPy.
- Have at least 5 GB of free space in your computer.
- While it is not required to have experience using Jupyter Notebooks, this would be very beneficial for the session.

What this tutorial is not

- A deep dive into Natural Language Processing.
- A deep learning tutorial.
- A web application tutorial.


## Setup

You should first make sure you have [Anaconda](https://www.anaconda.com/products/individual#download-section) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed. This will allow you to have most of the packages you will need for this session already installed once you open up Jupyter Lab.

Here are some of the ways in which you can get the setup for the tutorial ready.

### Option 1

#### First Step

Open up your terminal and navigate to a directory of your choosing in your computer. Once there, run the following command.

```sh
 git clone https://github.com/ramonpzg/db_training.git
```

Conversely, you can click on the green `download` button at the top and donwload all files to your desired folder/directory. Once you download it, unzip it and move on to the second step.

#### Second Step

To get all dependancies, packages and everything else that would be useful in this tutorial, you can recreate the environment by first going into the directory for today

```sh
cd db_training
```

and then running

```sh
conda env create -f environment.yml
```

#### Third Step

Then you will need to activate your environment using the following command.

```sh
conda activate vector
```

#### Fourth Step

Open up Jupyter Lab and you should be ready to go.

```sh
jupyter lab
```



### Option 2

#### First Step

Download the repo using the big green button on the upper right.

![green button](images/repo.png)

#### Second Step

Open a Jupyter Lab session inside the folder you just downloaded. You can do this through the Anaconda graphical user interface if you are on a Mac or Windows.

```sh
cd db_training
jupyter lab
```

Conversely, open a Jupyter Lab session anywhere you'd like and navigate to the folder you just downloaded.

#### Third Step

Open up a terminal inside of Jupyter Lab and run either of the following commands.

```sh
## one option
pip install arrow-cpp pyarrow bokeh holoviews matplotlib numba numpy pandas panel param parquet-cpp scikit-image scikit-learn scipy gensim pyldavis spacy spacy-alignments spacy-transformers datasets



## another option
conda install arrow-cpp pyarrow bokeh holoviews matplotlib numba numpy pandas panel param parquet-cpp scikit-image scikit-learn scipy gensim pyldavis spacy spacy-alignments spacy-transformers datasets -c conda-forge
```


If you receive an error while trying to install all packages, close out of jupyter lab, shut down your serrver, and follow the steps below.

```sh
## create an environment
conda create --name my_env_name python=3.9 pip

## activate your environment
conda activate my_env_name

## install some packages
pip install -U arrow-cpp pyarrow bokeh holoviews matplotlib numba numpy pandas panel param parquet-cpp scikit-image scikit-learn scipy gensim pyldavis spacy spacy-alignments spacy-transformers datasets

## open up jupyter lab
jupyter lab
```

Great work! Now navigate to lesson.ipynb and open it.


## Additional Resources

Here are a few great resources to get started with natural language processing data analytics, data visualisation, and dashboard creation. The first three, in particular, have guided my thinking and helped very much polished the content you have found in this tutorial.

- [Natural Language Processing in Action](https://www.manning.com/books/natural-language-processing-in-action) by Hobson Lane, Cole Howard, and Hannes Hapke
- [Learning Spark: Lightning-Fast Data Analytics](https://databricks.com/p/ebook/learning-spark-from-oreilly) by Jules S. Damji, Brooke Wenig, Tathagata Das, and Danny Lee
- [Fundamentals of Data Visualisation](https://clauswilke.com/dataviz/) by Claus O. Wilke
- [The Big Book of Dashboards](http://bigbookofdashboards.com/) by Steve Wexler, Jeffrey Shaffer, and Andy Cotgreave
- [# Practical Statistics for Data Scientists: 50+ Essential Concepts Using R and Python](https://www.amazon.com.au/Practical-Statistics-Data-Scientists-2e/dp/149207294X/ref=sr_1_1?dchild=1&keywords=Practical+Statistics+for+Data+Scientists+second+edition&qid=1624278273&s=books&sr=1-1) by Peter Bruce, Andrew Bruce, and Peter Gedeck
- [Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython](https://www.amazon.com/gp/product/1491957662/ref=as_li_qf_asin_il_tl?ie=UTF8&tag=quantpytho-20&creative=9325&linkCode=as2&creativeASIN=1491957662&linkId=ea8de4253cce96046e8ab0383ac71b33) by Wes McKinney

## Feedback 😃

If you liked or disliked this session and would like to give me your feedback so that I can improve it, I would greatly appreciate that.

> # [Feedback Form](https://docs.google.com/forms/d/e/1FAIpQLSft5_3bja48Hb0tRVqDUP5m4MBFyiL-jWx-lYA8B5-halY1zw/viewform?usp=sf_link)
