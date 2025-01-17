---
layout: default
img: for_the_sake_of_argument.png
caption: Identifying supporting and opposing arguments is a great way to annoy your friends.
img_link: https://xkcd.com/1432/
title: HW11 - Perspective Detection
active_tab: homework
release_date: 2020-04-15
due_date: 2020-04-22T23:59:59EDT
submission_link: 
attribution: This assignment was developed by Sihao Chen and Chris Callison-Burch for UPenn's CIS 530 class in Spring 2020 during the Coronavirus pandemic.
materials:
    - 
      name: Skeleton colab notebook (Please import this to colab)  
      url: perspective_hw.ipynb
readings:
-
   title: BERT&colon; Pre-training of Deep Bidirectional Transformers for Language Understanding
   authors: Jacob Devlin
   venue: Guest Lecture for CIS 530, Spring 2019
   type: Guest Lecture
   url: https://upenn.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=ebf01726-bd73-45f9-81d6-a9d6000a4c4e
- 
   title: BERT&colon; Pre-training of Deep Bidirectional Transformers for Language Understanding
   authors: Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova
   venue: NAACL
   type: conference
   year: 2019
   url: https://www.aclweb.org/anthology/N19-1423/
   page_count: 8
   id: bert
   abstract: We introduce a new language representation model called BERT, which stands for Bidirectional Encoder Representations from Transformers. Unlike recent language representation models, BERT is designed to pre-train deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task-specific architecture modifications. BERT is conceptually simple and empirically powerful. It obtains new state-of-the-art results on eleven natural language processing tasks, including pushing the GLUE score to 80.5% (7.7% point absolute improvement), MultiNLI accuracy to 86.7% (4.6% absolute improvement), SQuAD v1.1 question answering Test F1 to 93.2 (1.5 point absolute improvement) and SQuAD v2.0 Test F1 to 83.1 (5.1 point absolute improvement).
   bibtex: |
      @article{devlin2018bert,
        title={Bert&colon; Pre-training of deep bidirectional transformers for language understanding},
        author={Devlin, Jacob and Chang, Ming-Wei and Lee, Kenton and Toutanova, Kristina},
        journal={arXiv preprint arXiv:1810.04805},
        year={2018}
      }
-
   title: Seeing Things from a Different Angle&colon; Discovering Diverse Perspectives about Claims
   authors: Sihao Chen, Daniel Khashabi, Wenpeng Yin, Chris Callison-Burch and Dan Roth
   venue: NAACL
   type: conference
   year: 2019
   url: https://www.cis.upenn.edu/~ccb/publications/discovering-diverse-perspectives.pdf
   page_count: 16
   id: discovering-diverse-perspectives
   abstract: One key consequence of the information revolution is a significant increase and a contamination of our information supply. The practice of fact checking won’t suffice to eliminate the biases in text data we observe, as the degree of factuality alone does not determine whether biases exist in the spectrum of opinions visible to us. To better understand controversial issues, one needs to view them from a diverse yet comprehensive set of perspectives. For example, there are many ways to respond to a claim such as “animals should have lawful rights”, and these responses form a spectrum of perspectives, each with a stance relative to this claim and, ideally, with evidence supporting it. Inherently, this is a natural language understanding task, and we propose to address it as such. Specifically, we propose the task of substantiated perspective discovery where, given a claim, a system is expected to discover a diverse set of well-corroborated perspectives that take a stance with respect to the claim. Each perspective should be substantiated by evidence paragraphs which summarize pertinent results and facts. We construct PERSPECTRUM, a dataset of claims, perspectives and evidence, making use of online debate websites to create the initial data collection, and augmenting it using search engines in order to expand and diversify our dataset. We use crowdsourcing to filter out the noise and ensure high-quality data. Our dataset contains 1k claims, accompanied with pools of 10k and 8k perspective sentences and evidence paragraphs, respectively. We provide a thorough analysis of the dataset to highlight key underlying language understanding challenges, and show that human baselines across multiple subtasks far outperform machine baselines built upon state-of-the-art NLP techniques. This poses a challenge and opportunity for the NLP community to address.
   bibtex: |
      @inproceedings{Chen-et-al:2019:NAACL,
       author = {Sihao Chen and Daniel Khashabi and Wenpeng Yin and Chris Callison-Burch and Dan Roth},
       title = {Seeing Things from a Different Angle&colon; Discovering Diverse Perspectives about Claims},
       booktitle = {The 2019 Conference of the North American Chapter of the Association for Computational Linguistics (NAACL 2019)},
       month = {June},
       year = {2019},
       address = {Minneapolis, Minnesota},
       url = {http://www.cis.upenn.edu/~ccb/publications/discovering-diverse-perspectives.pdf}
       } 
-
   title: PerspectroScope&colon; A Window to the World of Diverse Perspectives
   authors: Sihao Chen, Daniel Khashabi, Chris Callison-Burch and Dan Roth
   venue: ACL
   type: demo
   year: 2019
   url: https://www.cis.upenn.edu/~ccb/publications/perspectroscope-demo.pdf
   page_count: 6
   id: perspectroscope-demo
   abstract: This work presents PERSPECTROSCOPE, a web-based system which lets users query a discussion-worthy natural language claim, and extract and visualize various perspectives in support or against the claim, along with evidence supporting each perspective. The system thus lets users explore various perspectives that could touch upon aspects of the issue at hand. The system is built as a combination of retrieval engines and learned textual entailment-like classifiers built using a few recent developments in natural language understanding. To make the system more adaptive, expand its coverage, and improve its decisions over time, our platform employs various mechanisms to get corrections from the users. PERSPECTROSCOPE is available at github.com/CogComp/perspectroscope.  A brief video of the system is available at youtube.com/watch?v=MXBTR1Sp3Bs.
   bibtex: |
      @inproceedings{Chen-Khashabi-et-al:2019,
       author = {Sihao Chen and Daniel Khashabi and Chris Callison-Burch and Dan Roth},
       title = {PerspectroScope&colon; A Window to the World of Diverse Perspectives},
       booktitle = {Proceedings of The 57th Annual Meeting of the Association for Computational Linguistics (ACL) demo session},
       year = {2019},
       address = {Florence, Italy},
       url = {http://www.cis.upenn.edu/~ccb/publications/comparison-of-diverse-decoding-methods-from-conditional-language-models.pdf}
      } 
---

<!-- Check whether the assignment is up to date -->
{% capture this_year %}{{'now' | date: '%Y'}}{% endcapture %}
{% capture due_year %}{{page.due_date | date: '%Y'}}{% endcapture %}
{% if this_year != due_year %} 
<div class="alert alert-danger">
Warning: this assignment is out of date.  It may still need to be updated for this year's class.  Check with your instructor before you start working on this assignment.
</div>
{% endif %}
<!-- End of check whether the assignment is up to date -->

<div class="alert alert-info">
This assignment is due before {{ page.due_date | date: "%I:%M%p" }} on {{ page.due_date | date: "%A, %B %-d, %Y" }}.
</div>

Perspective Detection <span class="text-muted">: Assignment 11</span>
=============================================================

When you ask Google question in natural language it attempts to get you a single correct answer.  This is great for questions like _What temperature is recommended for salmon?_ but it fails on questions for which there isn't a single correct answer like _Should uniforms be required in schools?_:


<table>
  <tr>
    <td>
      <div class="text-center">
      <img src="salmon.png" alt="Q: What temperature is recommended for salmon? A: 145 degrees Fahernheit." class="img-fluid" width="400px"  />
      </div>
  </td>
  <td>
    <div class="text-center" >
      <img src="school-uniforms.png" alt="Q: Should uniforms be required in schools? A: 145 degrees Fahernheit." class="img-fluid" width="400px"  />
    </div>
  </td>
</tr>
</table>

  

In questions like _Should uniforms be required in schools?_, users are seeking multiple perspectives on a topic.  Ideally, we should organize potential answers to such perspective-seeking queries into two sets: perspctives that support an idea, and perspectives that refute it.  

As part of his PhD research, your TA Sihao built a demonstration search engine called [PerspectroScope](https://perspectroscope.seas.upenn.edu/). Given a __claim__ as input, PerspectroScope will look for potential __perspectives__ on the web, and use classifiers trained on a dataset called [Perspectrum](https://cogcomp.seas.upenn.edu/perspectrum/) to decide whether each potential perspctive is __relevant__ and whether it is __supports__ or __opposes__ the claim.   Here's an example of Sihao's search engine organizes perspectives related to animal rights:

<div class="text-center">
<img src="perspectrum_eval_setting.png" alt="An overview of how a search engine could classify perspectives." class="img-fluid" width="500px"  />
</div>

Here is a [youtube video](https://www.youtube.com/watch?v=MXBTR1Sp3Bs) that demonstrates the functionality of the search engine. You are also welcomed to [try the search engine yourself](https://perspectroscope.seas.upenn.edu/).


### Learning Goals

The learning goals for this assignment are: 
- An introduction to **BERT**, which is a powerful architecture that can be used to solve many NLP tasks.  BERT is a large, pre-trained neural language model based on the Transformer architecture that can adapted to many classification tasks.
- Learn how to solve sentence pair **classification tasks by "fine-tuning" BERT** to the task.  The process of fine-tuning adapts a general pre-trained model like BERT to a specific task that you're interested in.
- We're going to fine-tune BERT to do two important classification tasks that play a part of the perspective search engine:
1. **Relevance Classification**: Given a claim and a perspective sentence, classify whether the sentence presents a **relevant perspective** to the claim.
2. **Stance Classification** (extra credit): Given a claim and a sentence of relevant perspective, classify whether the perspective **supports or refutes** the claim.

<!--
 (Extra credit) learn how to build your own _argument search engine_, if you are interested!  This is a current research topic in the field of NLP.  The goal is to allow people to search for multiple perspectives on a debatable topic like "uniforms should be worn in schools".
!-->


<!-- List the materials from the header -->
{% if page.materials %}
<div class="alert alert-info">
You can download the materials for this assignment here; The datasets will be downloaded via the Colab notebook.
<ul>
{% for item in page.materials %}
<li><a href="{{item.url}}">{{ item.name }}</a></li>
{% endfor %}
</ul>
</div>
{% endif %}

## Background: BERT

For this assignment, we are going to use BERT. 
BERT is a state-of-the-art neural language model that was released in 2019 by Google Research. BERT is an acronym for Bidirectional Encoder Representations from Transformers.  It can be used as an encoder to produce sentence embeddings, and to produce context-based word embeddings.   Models trained using BERT embeddings (or variants of BERT) have been producing state-of-the-art results across most NLP task recently. 

Like the word embeddings (e.g. Word2Vec, GloVe) that you have played with in a few of the past homework assignments, BERT is trained with similar, but slightly more sophisticated learning objectives -- The first objective is known as **Masked Language Modeling (MLM)**, where we randomly "mask" a certain fraction of words from a text during training and have the model predict the masked words. The second task objective **Next Sentence Prediction (NSP)** -- given two sentences, predict whether the second sentence comes after the first sentence in natural text. 

There are several things that make BERT so good: 

1. **Contextual**: A key difference between word embeddings and BERT is that BERT is contextual, which means it is producing embedding based on not only the word itself, but also the context it appears in. That way, the BERT embedding for each word is "dynamic", and will change based on the context it appears in. Such features allow BERT to capture various linguistics phenomena like word sense disambiguation. 
<!--
A [paper](https://nlp.stanford.edu/pubs/hewitt2019structural.pdf) in 2019, published by John Hewitt (an undergrad alumni of Professor Callison-Burch) et. al., found that BERT embedding itself encodes dependency parse structure of sentences.
-->

2. **Number of Parameters and Scale of Training**: BERT is huge. The base version of BERT (12 layers of transformers) consists of 110M parameters, and is trained on 800,000,000 words. 

3. **Fine-tuning**: Fine-tuning is a process to take a machine learning model that has already been trained for a given task/objective, and further train the model with a second similar task/objective. When you train models with BERT embeddings for downstream tasks, the entire BERT model's weights are updated during training, and so the BERT embeddings are "adapted" according to the task at hand. On contrary, when you use word embedding, you don't actually update the part of the network that was used to train the word embeddings. This process is called "BERT fine-tuning". The ability of fine-tuning makes BERT more expressive, and easier to adapt to the task-specific supervision. In this homework we will show you a step-by-step process of BERT fine-tuning.

<div class="alert alert-info" markdown="1">
For more information on BERT, we recommend watching [this guest lecture for CIS 530 by Jacob Devlin from Spring 2019](https://upenn.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=ebf01726-bd73-45f9-81d6-a9d6000a4c4e).  Jacob was the lead author on the [original BERT paper](https://www.aclweb.org/anthology/N19-1423/).
</div>


<!-- for a variety of natural language processing tasks belong to the *Transformer Family*, which are models based off of the Transformer architecture. The Transformer can be thought of as a big feed-forward network, with some fancy bells and whistles such as the attention mechanism. You might be wondering: why are we moving back to serial networks after such successes with RNNs and LSTMs? It turns out that although recurrent models are naturally poised to handle sequences as inputs, their non-serial nature makes them difficult to train in a distributed/parallel fashion. This means that serial networks can be trained faster, unlocking new orders of magnitude of data to use as training data. Some examples of notable state-of-the-art Transformer based models are Open AI’s GPT-2 and in this homework, Google’s BERT. -->
<!-- BERT is an extremely influential model and stands for Bidirectional Encoder Representations from Transformers.  and with hundreds of millions of parameters, it is a large and powerful neural network for predicting the probabilities of natural language - otherwise known as a *language model* (recall Homeworks 3 and 6). Similar to Word2Vec’s negative sampling technique, we train the model using different objectives, learning efficient *embeddings* along the way.  In addition, the model serves as a vessel for *transfer learning*, where we can use a pre-trained instance of BERT and *fine-tune* the model on additional training data to better serve a certain domain of text. -->

### Sentence Pair Classification

Sentence pair classification is the task of classifying what relation holds between a pair of sentences. Many popular tasks in NLP can be viewed as examples of sentence pair classification. E.g. Almost every task in the [GLUE Benchmark](https://gluebenchmark.com/leaderboard) -- a collection of datasets for evaluating a model's capability of "language understanding".

BERT has been shown to be very effective for sentence pair classification. For the rest of this homework, we are going to introduce and work on one of such tasks as example.



## Part 1: Relevance Classification via BERT fine-tuning 
For this part, we will show you how to build a BERT-based sentence pair classifer for Perspective Relevance Classification.

To help you understand what the task is about. Here's an example in `perspectrum_train.json`: For each given claim, there are a few perspectives that either supports or refutes the claim. **All these "perspectives" are relevant arguments to the claim**. However, if you are building an search engine that searches for such perspectives on the open web, you will be needing a classfier, which, given a claim, can detect whether a sentence is a relevant argument to the claim or not. Note that a challenge here is -- we don't have negative examples provided. So we will be doing negative sampling to get unrelated perspectives for training. 

```
{
    "cid": 188,
    "claim_text": "We must grant those diagnosed with terminal illnesses the right to access treatments that have not completed clinical testing",
    "perspective_for": [
        {
            "id": 1397,
            "text": "It is cruel to deny people the last hope"
        },
        {
            "id": 22189,
            "text": "It is amoral to deny terminal patients last hope treatments"
        },
        ...
    ],
    "perspective_against": [
        {
            "id": 1400,
            "text": "This gives people false hope"
        },
        {
            "id": 22193,
            "text": "Terminally ill patients would be getting false hope"
        },
        ...
    ]
}
``` 

We would like you to follow the notebook, and understand how each step works when training (or fine-tuning) a BERT-based sentence pair classifier for the task. Roughly there are 5 steps to the whole procedure. The code for step 1-4 is already given to you in the notebook. You will need to implement the last step, which should be very similar to step 4. 
1. Convert the training dataset into sentence pair format. Sample negative examples (i.e. arguments/perspectives not relevant to the input claim) for training.
2. Preprocess data and extract features as input to BERT
3. Intialize BERT model and Fine-tune BERT with positive and negative sentence pairs
4. Evaluate on the dev set to get a performance of the model
5. Predict on the test set, where the labels are hidden from you. 

The goal for this part is to get yourself familiar with PyTorch/BERT through examples. These steps are common to developing Neural Network models for most sentence-level NLP tasks, and should give you a general idea on how you would train/evaluate a BERT-based classifier. Feel free to improve or build upon the example code if you are interested in using it for other tasks.  

Follow instructions and submit your model's prediction on the test data; store the predictions in a file named `relevance_test_predictions.txt`, and submit the file. 

**Important Note**: the labels of the test data are NOT given to you in this homework. However the helper functions will still generate a dummy label for each input sentence pair. The only way to measure the correct accuracy on test set is submitting your test results `relevance_test_predictions.txt` to Gradescope. 

## Part 2: DIY - Stance Classification (Optional, Extra Credit)
Now that you have seen an example, and hopefully are becoming an expert of BERT, let's try to follow similar steps and tackle the stance classification. Given a claim and a relevant perspective, classify whether the perspective supports or refutes the claim. 

For the most part we expect you to be re-using code from Part 1. Since this is a different task, you will be doing step 1 (generating positive and negative sentence pairs) in a slightly different way; Specifically  --

1.   In `perspectrum_train.json`, for each given claim, both supporting and refuting perspectives have been given to you. So you don't need to do negative sampling. Instead you should take the claim + "supporting" perspective as positive sentence pair and claim with "refuting" perspective as negative pair.   

2.   The task assumes that for every input claim-perspective pair, the perspective is relevant to the claim. So when generating training pairs, you should make sure of that.

Submit your model's prediction on the test data; store the predictions in a file named `stance_test_predictions.txt`, and submit the file.

## Part 3: Improving your classifier(s)
The model setup provided in the default skeleton will not give you nice results on the test set. For this part, we would like you to implement at least **three types of modifications/additions** to the provided baseline, and **include your findings (e.g. results on dev set) in the final report**.

There are leaderboards for both relevance and stance classification tasks. Please submit `relevance_test_predictions.txt` (**required**) and (optional) `stance_test_predictions.txt`  for entry to the leaderboard, and see your score on the test set.

Here are **some ideas for improvements**:

1. **Increase the number of transformer layers for BERT**. In the colab notebook, we are using a mini version of BERT, which consists of 4 layers of transformer. The base version of BERT has 12 layers, which will give way better performance, at the cost of longer training/evaluation time.
2. **Use other variants of BERT** (E.g. ALBERT, RoBERTa). You can find a more-than-enough list of available models from the [README](https://github.com/huggingface/transformers) of huggingface transformer package.
3. For the relevance classification task, you can adopt **better negative sampling strategies** for training -- We've previously ask you to sample negative examples randomly. For example, a better negative example would be, perspectives not related to the claim, but have significant word overlap (e.g. it's discussing similar topics, but it's not an valid argument towards the claim). 
4. **Parameter Tuning**: In the skeleton code, we have listed a suggested range of hyperparameter (e.g. different learning rates and batch sizes). You are welcomed to try different values for each hyperparameter, and report your findings!

## Report

As usual we want you to keep track of all experiments and findings in your report. But here are the list of things that we are looking for (and will grade the report on).
1. You should make **at least three modifications/extension** to the baseline model and explain what you did. 
2. For each modification, specify the size and the type of the BERT model you use, plus the hyper-parameters you chose for training. Include the performance on the dev set for each configuration.
3. Using the best performing model on dev set, identify a few mistakes that the model makes on dev set. Include a few of such claim/perspective pairs in the report and briefly describe the mistake and why you think the model produces the wrong prediction.
4. **Write a few sentences on what you think makes the Perspective Detection task challenging**. (Note that there isn't a single correct answer to the question; we are interested in knowing your perspective!)


## Deliverables 
<div class="alert alert-warning" markdown="1">
Here are the deliverables that you will need to submit:
* Your notebook, downloaded and named as `perspectrum.py`. You can download your notebook as a `.py` file by going to the menu bar: "File" -> "Download .py".
* Results on the test sets of Relevance or Stance classification task, named `relevance_test_predictions.txt` and `stance_test_predictions.txt` respectively.
* PDF Report (called writeup.pdf)
</div>

## Recommended readings

<table>
   {% for publication in page.readings %}
    <tr>
      <td>
	{% if publication.url %}
		<a href="{{ publication.url }}">{{ publication.title }}.</a>
        {% else %}
		{{ publication.title }}.
	{% endif %}
	{{ publication.authors }}.
	{{ publication.venue }}  {{ publication.year }}.

	{% if publication.abstract %}
	<!-- abstract button -->
	<a data-toggle="modal" href="#{{publication.id}}-abstract" class="label label-success">Abstract</a>
	<!-- /.abstract button -->
	<!-- abstract content -->
	<div id="{{publication.id}}-abstract" class="modal fade" tabindex="-1" role="dialog" aria-labelledby="{{publication.id}}">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title" id="{{publication.id}}">{{publication.title}}</h4>
        </div><!-- /.modal-header -->
        <div class="modal-body">
        {{publication.abstract}}
        </div><!-- /.modal-body -->
	</div><!-- /.modal-content -->
	</div><!-- /.modal-dialog -->
	</div><!-- /.abstract-content -->
	{% endif %}
		{% if publication.bibtex %}
	<!-- bibtex button -->
	<a data-toggle="modal" href="#{{publication.id}}-bibtex" class="label label-default">BibTex</a>
	<!-- /.bibtex button -->
	<!-- bibtex content -->
	<div id="{{publication.id}}-bibtex" class="modal fade" tabindex="-1" role="dialog" aria-labelledby="{{publication.id}}">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title" id="{{publication.id}}">{{publication.title}}</h4>
        </div><!-- /.modal-header -->
        <div class="modal-body">
 	   <pre>{{publication.bibtex}}
           </pre>
        </div><!-- /.modal-body -->
	</div><!-- /.modal-content -->
	</div><!-- /.modal-dialog -->
	</div><!-- /.bibtex-content -->
	{% endif %}
</td></tr>
  {% endfor %}
</table>


