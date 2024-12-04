# Using huggingface and elasticsearch to see how the internet feels

One of the benefits of new social media platforms focusing on principles like opensource and decentralization is that we're also getting more easily accessible data to play with.

This project will explore one of [the newest Hugging Face datasets](https://huggingface.co/datasets/alpindale/two-million-bluesky-posts) of 2 million bluesky posts. With the use of elasticsearch and models from the HF hub we can build some interesting queries to take the pulse of the internet.

Using [a sentiment analysis model](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment) we can classify posts into `negative`, `positive`, or `neutral`.
Adding that to the rest of the classic search features like `filtering`, `scoring`, or `matching` lets us explore social activity in a comprehensice (and fun!) way.

Questions to look at:
* What are trends regarding sentiment & posts? Do we get more negative or positive posts? 
* Which topics are currently trending? 
* Deeper dive into particular topics and how users feel about it (like puppies or maybe other social media platforms?)
* Do trends or feelings change over time?

and more!

## Overview

[The first notebook](/huggingface_dataset_search.ipynb) starts from the HuggingFace dataset and begins with some simple searches

[The second notebook](/elasticsearch_with_huggingface.ipynb) builds an inference pipeline to enrich our data with sentiment labels

TBD - we can now answer some of our questions by building some complex queries and visualizing our data in Kibana 
