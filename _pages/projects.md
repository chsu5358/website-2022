---
layout: page
title: Projects
permalink: /projects/
description:
nav: true
dropdown: true
children: 
    - title: Multi-facet Embedding for Language Modeling
      permalink: /projects/#header-multifacet-embedding-LM
    - title: Active Learning and Crowdsourcing
      permalink: /projects/#header-active-learning
    - title: Natural Language Processing
      permalink: /projects/#header-NLP
    - title: Computer Vision (Clustering and Matching)
      permalink: /projects/#header-CV

display_categories: [Multi-facet Embedding for Language Modeling, Active Learning and Crowdsourcing, Natural Language Processing, Computer Vision (Clustering and Matching)]
#display_categories: [Natural language processing, Neural network, Education, Computer vision and multimedia]
horizontal: false
display_grids: false
nav_order: 2
---
<!--
<div class="row row-grid">
  <h4></h4>
  <div class="col-6">
    <img src="../assets/img/" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    </p>
  </div>
</div>
-->

<!-- 02.22[CY] -->
<div class="div-cat-header">
  <h2 id="header-multifacet-embedding-LM">Multi-facet Embedding for Language Modeling</h2>
</div>

<h4>Why Multiple Embeddings are Better in LM's Output Softmax Layer</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/Multi-facet_Softmax.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      We theoretically show that this single hidden state cannot produce all probability distributions regardless of the language model (LM) size or training data size because the single hidden state embedding cannot be close to the embeddings of all the possible next words simultaneously when there are other interfering word embeddings between them. Our work not only deepens our understanding of softmax bottleneck and mixture of softmax (MoS) but also inspires us to propose multi-facet softmax (MFS) to address the limitations of MoS (<a href="https://openreview.net/forum?id=n0jZ0QyXzj">Paper</a>).
    </p>
  </div>
</div>


<h4>Predicting the Future Topics for Interactive Language Generation</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj1-nlp-interactive_LM_first_figure.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      We design a framework that displays multiple candidate upcoming topics, of which a user can select a subset to guide the generation. Our framework consists of two components: (1) a method that produces a set of candidate topics by predicting the centers of word clusters in the possible continuations, and (2) a text generation model whose output adheres to the chosen topics. The training of both components is self-supervised, using only unlabeled text. Our experiments demonstrate that our topic options are better than those of standard clustering approaches, and our framework often generates fluent sentences related to the chosen topics, as judged by automated metrics and crowdsourced workers
      (<a href="http://arxiv.org/abs/2103.15335">Paper</a>, <a href="https://github.com/iesl/interactive_LM">Code</a>, <a href="https://slideslive.com/38954487/changing-the-mind-of-transformers-for-topicallycontrollable-language-generation">Talk</a>, <a href="../assets/pdf/proj1-nlp-interactive_LM-EACL_interactive_LM-slides.key" download="slides-eacl2021-Changing the Mind of Transformers for Topically-Controllable Language Generation">Slides</a>, <a href="../assets/pdf/proj1-nlp-interactive_LM-EACL_interactive_LM-poster.pdf" download="poster-eacl2021-Changing the Mind of Transformers for Topically-Controllable Language Generation">Poster</a>).
    </p>
  </div>
</div>


<h4>Multi-facet Embeddings for Distantly Supervised Relation Extraction</h4>
<div class="row row-grid">  
  <div class="col-6">
    <img src="../assets/img/proj2-nlp-Multi-facet Embeddings for Relation Extraction.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      We propose multi-facet universal schema that uses a neural model to represent each sentence pattern as multiple facet embeddings and encourage one of these facet embeddings to be close to that of another sentence pattern if they cooccur with the same entity pair. In our experiments, we demonstrate that multi-facet embeddings significantly outperform their single facet embedding counterpart, compositional universal schema (Verga et al., 2016), in distantly supervised relation extraction tasks. Moreover, we can also use multiple embeddings to detect the entailment relation between two sentence patterns when no manual label is available
      (<a href="http://arxiv.org/abs/2103.15339">Paper</a>, <a href="https://github.com/rohanpaul11/multifacet-re">Code</a>, <a href="https://slideslive.com/38954382/multifacet-universal-schema">Talk</a>, <a href="../assets/pdf/proj2-nlp-Multi-facet RE-EACL_multi-facet_RE_small-slides.key" download="slides-eacl2021-Multi-facet Universal Schema">Slides</a>, <a href="../assets/pdf/proj2-nlp-Multi-facet RE-EACL_multi-facet_RE_small-poster.pdf" download="poster-eacl2021-Multi-facet Universal Schema">Poster</a>).
    </p>
  </div>
</div>

<h4>Predicting Cluster Centers for Sentence Representation</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj3-nlp-Multi-facet Embeddings for Sentence Representation.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      We propose a novel embedding method for a text sequence (e.g., a sentence) where each sequence is represented by a distinct set of multi-mode codebook embeddings to capture different semantic facets of its meaning. The codebook embeddings can be viewed as the cluster centers which summarize the distribution of possibly co-occurring words in a pre-trained word embedding space. Our experiments show that the per-sentence codebook embeddings significantly improve the performances in unsupervised sentence similarity and extractive summarization benchmarks (<a href="http://arxiv.org/abs/2103.15330">Paper</a>, <a href="https://docs.google.com/presentation/d/1k-OBWdBYsGmXUuvNc1_J_JrEppB_Aqh82bJPCgjFL-s/edit?usp=sharing">Slides</a>, <a href="../assets/pdf/proj3-nlp-Multi-facet Embeddings for Sentence Representation-poster.pdf" download="poster-aaai2021-Extending Multi-sense Word Embedding to Phrases and Sentences for Unsupervised Semantic Applications">Poster</a>). 
    </p>
  </div>
</div>

<br>
<hr>
<div class="div-cat-header">
  <h2 id="header-active-learning">Active Learning and Crowdsourcing</h2>
</div>

<h4>Overcoming Practical Issues of Deep Active Learning</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj4-nlp-Overcoming Practical Issues of Deep Active Learning.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      Existing deep active learning algorithms achieve impressive sampling efficiency on natural language processing tasks. However, they exhibit several weaknesses in practice, including (a) inability to use uncertainty sampling with black-box models, (b) lack of robustness to noise in labeling, (c) lack of transparency. In response, we propose a transparent batch active sampling framework by estimating the error decay curves of multiple feature-defined subsets of the data. We perform extensive experiments on four named entity recognition (NER) tasks and results show that our methods greatly alleviate these limitations without sacrificing too much sampling efficiency 
      (<a href="https://arxiv.org/abs/1911.07335">Paper</a>, <a href="https://slideslive.com/38933012/using-error-decay-prediction-to-overcome-practical-issues-of-deep-active-learning-for-named-entity-recognition">Slides</a>, <a href="https://slideslive.com/38933012/using-error-decay-prediction-to-overcome-practical-issues-of-deep-active-learning-for-named-entity-recognition">Talk</a>).
    </p>
  </div>
</div>


<h4>Active Sampling for Estimating Quality of Experience (QoE) Model</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/active_QoE.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    We use Bayesian learning to model the non-linear relationships between quality of experience (QoE) and multiple factors.
    </p>
    <p>
    Our experiment shows that active sampling can be used to reduce the number of samples collected from crowdsourcing for building the model, but the users' perception of the video quality would be affected by the active learning methods (<a href="../assets/pdf/proj9-cv-Active Sampling for estimating QoE model-paper.pdf" download="paper-ieee trans. multimed. 2018-Active learning for crowdsourced QoE modeling">Paper</a>).
    </p>
  </div>
</div>

<h4>Student Modeling and Prerequisite Verification in Knowledge Tree</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj8-education-student modeling.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    We extract answering logs of the exercises from <a href="https://www.junyiacademy.org/">Junyi Academy</a>, an E-learning website similar to Khan Academy.
    </p>
    <p>
    We use crowdsourcing and machine learning to discover prerequisite relationships between exercises. Based on that, we design a mechanism of adaptive test to improve the learning experiences of Junyi academy (<a href="../assets/pdf/proj8-education-student modeling-paper.pdf" download="paper-edm2015-Modeling Exercise Relationships in E-Learning: A Unified Approach">Paper</a>, <a href="../assets/pdf/proj8-education-student modeling-presentation.pptx" download="slides-edm2015-Modeling Exercise Relationships in E-Learning: A Unified Approach">Presentation</a>, <a href="http://people.umass.edu/hawshiuancha/junyi_dependency_prediction.zip">Demo</a>, <a href="https://pslcdatashop.web.cmu.edu/DatasetInfo?datasetId=1198">Dataset</a>).
    </p>
  </div>
</div>

<h4>Emphasize Uncertain Examples in Supervised Learning</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj7-nn.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    Inspired by active learning, we propose two alternatives to re-weight training samples based on lightweight estimates of sample uncertainty in stochastic gradient descent (SGD). Experimental results on six datasets show that our methods reliably improve accuracy in various network architectures, including additional gains on top of other popular training techniques (<a href="https://arxiv.org/abs/1704.07433">Paper</a>, <a href="https://arxiv.org/abs/1704.07433">Poster</a>).
    </p>
  </div>
</div>

<br>
<hr>
<div class="div-cat-header">
  <h2 id="header-NLP">Natural Language Processing</h2>
</div>

<h4>Distributional Inclusion Vector Embedding for Unsupevised Hypernym Detection</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj5-nlp-DIVE.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      We propose a novel word embedding method that preserves the distributional inclusion property in the sparse-bag-of-word (SBOW) feature. The embedding can be used to predict the generality of words, detect the hypernym relation, and discover the topics from the raw text simultaneously. The extensive experiments show that the embedding effectively compresses the SBOW, and achieves new state-of-the-art performances on the unsupervised hypernym detection tasks (<a href="https://arxiv.org/abs/1710.00880">Paper</a>, <a href="https://github.com/iesl/Distributional-Inclusion-Vector-Embedding">Code</a>, <a href="https://bl.ocks.org/chsu5358/raw/f08d4755b0f04e113c139a72a977df5c/">Demo</a>, <a href="../assets/pdf/proj5-nlp-DIVE-poster.pdf" download="poster-naacl2018-Distributional Inclusion Vector Embedding for Unsupervised Hypernymy Detection">Poster</a>). We also show that DIVE could help us to do word sense induction more efficiently (<a href="https://arxiv.org/abs/1804.03257">Paper</a>, <a href="../assets/pdf/proj5-nlp-DIVE-slides.pdf" download="slides-TextGraphs2018-Efficient Graph-based Word Sense Induction by Distributional Inclusion Vector Embeddings">Slides</a>).
    </p>
  </div>
</div>

<h4>UMASS TAC-KBP 2016 System for Relation Extraction</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj6-nlp-UMASS TAC 2016.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
      TAC-KBP is one of the most challenging text-based information retrieval tasks. We integrate research that is done in UMASS IESL in the past year, including embedding linker, multilingual Universal Schema, and LSTM sentence embedding. We perform extensive error analysis and develop some novel techniques (such as using a search engine to reduce noise in training data) to tackle the problems (<a href="../assets/pdf/proj6-nlp-UMASS TAC 2016-paper.pdf" download="paper-tac2016-Extracting Multilingual Relations under Limited Resources">Paper</a>).
    </p>
  </div>
</div>


<hr>
<div class="div-cat-header">
  <h2 id="header-CV">Computer Vision (Clustering and Matching)</h2>
</div>

<h4>Hierarchical Image Segmentation without Training</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj10-cv-Hierarchical Image Segmentation without Training.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    We proposed a general framework that applies classifiers with different complexity to discriminate segments in an image.
    </p>
    <p>
    Our unsupervised hierarchical segmentation results achieve similar or better performance in several standard benchmarks compared with the current state-of-the-art methods based on supervised learning (<a href="../assets/pdf/proj10-cv-Hierarchical Image Segmentation without Training-paper.pdf" download="paper-accv2014-Simple-to-Complex Discriminative Clustering for Hierarchical Image Segmentation">Paper</a>, <a href="../assets/pdf/proj10-cv-Hierarchical Image Segmentation without Training-poster.pdf" download="poster-accv2014-Simple-to-Complex Discriminative Clustering for Hierarchical Image Segmentation">Poster</a>, <a href="http://mml.citi.sinica.edu.tw/papers/HDC_code_ACCV_2014/">Code</a>).
  </p>
  </div>
</div>

<h4>Decomposi-tion of Multiple Foreground Co-segmentation</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/MFC.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    We proposed an efficient algorithm that decomposes the unsupervised Multiple Foreground Co-segmentation problem into three sub-problems: segmentation, matching, and figure-ground classification.
    </p>
    <p>
    Our method improves the accuracy of the state-of-the-art method by 13% in a standard benchmark (<a href="../assets/pdf/proj11-cv-Decomposition of Multiple Foreground Co-segmentation-paper.pdf" download="paper-cviu2015-Optimizingthedecompositionformultipleforegroundcosegmentation">Paper</a>, <a href="http://mml.citi.sinica.edu.tw/papers/MFC_code_CVIU_2015">Code</a>).
    </p>
  </div>
</div>

<h4>Superpixel-Based Large Displacement Optical Flow</h4>
<div class="row row-grid">
  <div class="col-6">
    <img src="../assets/img/proj12-cv-Superpixel-Based Large Displacement Optical Flow.png" class="img-responsive" width="100%">
  </div>
  <div class="col">
    <p>
    We formulated our objective function at the superpixel level rather than the pixel level as the traditional optical flow method did.</p>
    <p>
    Our method achieves a better large displacement matching capability than LDOF in videos with lower quality (<a href="../assets/pdf/proj12-cv-Superpixel-Based Large Displacement Optical Flow-paper.pdf" download="paper-icip2013-SUPERPIXEL-BASED LARGE DISPLACEMENT OPTICAL FLOW">Paper</a>, <a href="../assets/pdf/proj12-cv-Superpixel-Based Large Displacement Optical Flow-poster.pdf" download="poster-icip2013-SUPERPIXEL-BASED LARGE DISPLACEMENT OPTICAL FLOW">Poster</a>, <a href="http://mml.citi.sinica.edu.tw/papers/SPLDOF_code.php">Code</a>).
    </p>
  </div>
</div>



<!-- [Grids] pages/projects.md -->
<div class="projects">
 {%- if page.display_grids %} 
  {%- if site.enable_project_categories and page.display_categories %}
    <!-- Display categorized projects -->
    {%- for category in page.display_categories %}
    <h2 class="category">{{ category }}</h2>
    {%- assign categorized_projects = site.projects | where: "category", category -%}
    {%- assign sorted_projects = categorized_projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-2">
      {%- for project in sorted_projects -%}
        {% include projects_horizontal.html %}
      {%- endfor %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {%- for project in sorted_projects -%}
        {% include projects.html %}
      {%- endfor %}
    </div>
    {%- endif -%}
    {% endfor %}

  {%- else -%}
  <!-- Display projects without categories -->
    {%- assign sorted_projects = site.projects | sort: "importance" -%}
    <!-- Generate cards for each project -->
    {% if page.horizontal -%}
    <div class="container">
      <div class="row row-cols-2">
      {%- for project in sorted_projects -%}
        {% include projects_horizontal.html %}
      {%- endfor %}
      </div>
    </div>
    {%- else -%}
    <div class="grid">
      {%- for project in sorted_projects -%}
        {% include projects.html %}
      {%- endfor %}
    </div>
    {%- endif -%}
  {%- endif -%}
{% endif %}
</div>
