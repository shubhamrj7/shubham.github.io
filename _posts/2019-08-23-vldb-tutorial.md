---
layout: post
title:  "VDLB 2019 Tutorial (Tutorial Page)"
date:   2019-08-23 10:00:00 -0400
tags: vldb tutorial 2019
---

### VLDB 2019 Tutorial:
<center>
<h1>
Tutorial 6: TextCube: Automated Construction and Multidimensional Exploration
</h1>
Yu Meng, Jiaxin Huang, Jingbo Shang, Jiawei Han<br/>
Computer Science Department, University of Illinois at Urbana-Champaign<br/>
Time: <b>2:00PM - 5:30PM, Aug 29, 2019</b><br/>
Location: <b>Avalon</b><br/>
</center>

## Slides

[Preliminary Version](https://www.dropbox.com/s/gbqd83zocy2szph/VLDB%2719%20tutorial.pdf?dl=1)

## Abstract

Today's society is immersed in a wealth of text data, ranging from news articles, to social media, research literature, medical records, and corporate reports. A grand challenge of data science and engineering is to develop effective and scalable methods to extract structures and knowledge from massive text data to satisfy diverse applications, without extensive, corpus-specific human annotations. 

In this tutorial, we show that TextCube provides a critical information organization structure that will satisfy such an information need. We overview a set of recently developed data-driven methods that facilitate automated construction of TextCubes from massive, domain-specific text corpora, and show that TextCubes so constructed will enhance text exploration and analysis for various applications. We focus on new TextCube construction methods that are scalable, weakly-supervised, domain-independent, language-agnostic, and effective (i.e., generating quality TextCubes from large corpora of various domains). We will demonstrate with real datasets (including news articles, scientific publications, and product reviews) on how TextCubes can be constructed to assist multidimensional analysis of massive text corpora.


## Outline

1. Introduction
    - Motivations & Prior Arts
    - Overview of Multidimensional Text Analysis
2. Phrase Mining
    - What are quality phrases?
    - Supervised Methods
        * Noun Phrase Chunking Methods
        * Parsing-based Methods
        * How to rank entities at the corpus-level?
    - Unsupervised Methods
        * Raw Frequency based Methods
        * Concordance based Methods
        * Topic Model based Methods
        * Comparative Methods
    - Weakly/Distantly Supervised Methods
        * Phrasal Segmentation and its Variants
        * How to leverage distant supervision?
    - System demos and software introduction
        * A multilingual phrase mining system which integrates [AutoPhrase](https://github.com/shangjingbo1226/AutoPhrase), [SegPhrase](https://github.com/shangjingbo1226/SegPhrase), and TopMine together and supports phrase mining in multiple languages (e.g., English, Spanish, Chinese, Arabic, and Japanese).
3. Text Representation
    - Unsupervised Word Embedding
        * Context-free representation
        * Contextualized representation
    - Other embeddings: Network embedding
        * DeepWalk, LINE, node2vec, ...
    - Category name-guided word embedding
        * CatE
    - System demos and software introduction
        * Our CatE system demo
4. Entity Recognition
    - What is named entity recognition?
    - Handcrafted Features + Human Supervision
        * Classical Models: Conditional Random Filed
        * Standford NER
        * Twitter NER
    - Automated Features + Human Supervision
        * LSTM-CRF, LSTM-CNN-CRF, ...
        * LM-LSTM-CRF, EMLo, Flair, ...
        * Multi-task learning
    - Automated Features + Distant Supervision
        * AutoEntity, SwellShark, ClusType, Distant-LSTM-CRF, ...
        * FuzzyCRF & AutoNER
    - System Demos and Software
        * Named entity recognition inference Python package: [LightNER](https://github.com/LiyuanLucasLiu/LightNER). This module helps users easily apply the pre-trained NER models to their own corpus in an efficient and portable manner.
5. Text Cube Construction
    - Taxonomy Basics and Construction
    - Cluster-based Taxonomy Construction
        * Hierarchical Topic Modeling
        * General Graphical Model Approach
        * Hierarchical Clustering
    - Text Cube Basics and Construction
        * What is Text Cube?
        * Automatic document allocation for Text Cube construction
    - System Demos and Software
        * Publication Dataset Analysis Demo
6.  Text Cube Exploration
    - Cube-based Multidimensional Analysis
        * Statistical Measures Aggregation
        * Phrase-based Cell Summarization
        * Key N-gram based Ranking and Exploration
    - System Demos and Software
        * Demo: MissionCube
6. Summary and Future Directions
    - Summary of Text Cube
        * Principles and Techniques
        * Advantages and Limitations
        * How to build a text cube based on your application?
    - Future Directions


## Presenters

<img align="left" img src="/img/BIO/yumeng.jpg" alt="Drawing" style="width: 200px;margin-right:50px;"/>**Yu Meng**, Ph.D. student, Computer Science, UIUC. His research focuses on mining structured knowledge from massive text corpora with minimum human supervision. 

<br/>
<br/>
<br/>
<br/>
<br/>

<img align="left" img src="/img/BIO/jiaxinhuang.jpg" alt="Drawing" style="width: 200px;margin-right:50px;"/>**Jiaxin Huang**, Ph.D. student, Computer Science, UIUC. Her research focuses on mining structured knowledge from massive text corpora. She is the recipient of Chirag Foundation Graduate Fellowship in Computer Science.

<br/>
<br/>

<img align="left" img src="/img/BIO/jingbo.jpg" alt="Drawing" style="width: 200px;margin-right:50px;margin-top:10px"/>**Jingbo Shang**, Ph.D. candidate, Department of Computer Science, Univ. of Illinois at Urbana-Champaign. His research focuses on mining and constructing structured knowledge from massive text corpora with minimum human effort. His research has been recognized by multiple prestigious awards, including Grand Prize of Yelp Dataset Challenge (2015), Google PhD Fellowships (2017-2019) on Structured Data and Database Management. Mr. Shang has rich experiences in delivering tutorials in major conferences (SIGMOD'17, WWW'17, SIGKDD'17, SIGKDD'18, SIGKDD'19).

<img align="left" img src="/img/BIO/hanj.jpg" alt="Drawing" style="width: 200px;margin-right:50px;"/>**Jiawei Han** is Abel Bliss Professor in the Department of Computer Science at the University of Illinois. He has been researching into data mining, information network analysis, and database systems, with over 600 publications. He served as the founding Editor-in-Chief of ACM Transactions on Knowledge Discovery from Data (TKDD). Jiawei has received ACM SIGKDD Innovation Award (2004), IEEE Computer Society Technical Achievement Award (2005), IEEE Computer Society W. Wallace McDowell Award (2009), and Daniel C. Drucker Eminent Faculty Award at UIUC (2011). He is a Fellow of ACM and a Fellow of IEEE. He is currently the Director of Information Network Academic Research Center (INARC) supported by the Network Science-Collaborative Technology Alliance (NS-CTA) program of U.S. Army Research Lab. His co-authored textbook ``Data Mining: Concepts and Techniques'' (Morgan Kaufmann) has been adopted worldwide.