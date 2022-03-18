---
layout: page
title: Software
permalink: /software/
description:
nav: true
display_categories: [Natural Language Processing, Computer Vision and Multimedia]
horizontal: false
display_grids: false
nav_order: 4
---
<!--
<div class="row row-grid">
  <h4></h4>
  <p>
  </p>
</div>
-->

<!-- 02.22[CY] -->
<div class="div-cat-header">
  <h2>Natural Language Processing</h2>
</div>
<div>
  <h4>Multi-facet Embeddings</h4>
  <div>
    <ul style="list-style-type:circle;">
      <li>Interactive Language Generation <a href="https://github.com/iesl/interactive_LM">(PyTorch and python)</a></li>
      <li>Multi-facet Relation Extraction <a href="https://github.com/rohanpaul11/multifacet-re">(PyTorch and python)</a></li>
    </ul>
  </div>
</div>

<div>
  <h4>Unsupervised Hypernym Detection</h4>
  <div>
    <ul style="list-style-type:circle;">
      <li>Distributional Inclusion Vector Embedding <a href="https://github.com/iesl/Distributional-Inclusion-Vector-Embedding">(tensorflow and python)</a></li>
    </ul>
  </div>
</div>

<div>
  <h4>Educational Data Mining</h4>
  <div>
    <ul style="list-style-type:circle;">
      <li>Demo code to visualize predicted exercise relationships <a href="">(GAE for python)</a></li>
    </ul>
  </div>
</div>
<br>

<!-- 02.22[CY] -->
<hr>
<div class="div-cat-header">
  <h2>Computer Vision and Multimedia</h2>
</div>

<div>
  <h4>Unsupervised Segmentation</h4>
  <div>
  <ul style="list-style-type:circle;">
    <li>Hierarchical Image Segmentation without Training <a href="http://mml.citi.sinica.edu.tw/papers/HDC_code_ACCV_2014/">(Matlab)</a></li>
    <li>Mutiple Foreground Cosegmentation Decomposition <a href="http://mml.citi.sinica.edu.tw/papers/MFC_code_CVIU_2015">(Matlab)</a></li>
    <li>Efficient Hierarchical Graph-based Video Segmentation <a href="http://mml.citi.sinica.edu.tw/papers/GBH_code_ACCV_2014">(C/C++ for Windows)</a></li>
    ~10 times faster than the original from <a href="https://cse.buffalo.edu/~jcorso/r/supervoxels/">LIBSVX</a>
  </ul>

  </div>
</div>

<div>
  <h4>Clustering</h4>
  <div>
  <ul style="list-style-type:circle;">
    <li>Efficient Kmeans Using Multiple Threads <a href="http://www.mathworks.com/matlabcentral/mlc-downloads/downloads/submissions/47737/versions/4/download/zip">(C/C++ with Matlab wrapper)</a></li>
    ~3 times faster than Matlab statistical toolbox<br>
    <li>Efficient GMM Using Multiple Threads <a href="http://www.mathworks.com/matlabcentral/mlc-downloads/downloads/submissions/47741/versions/2/download/zip">(C/C++ with Matlab wrapper)</a></li>
    ~6 times faster than Matlab statistical toolbox
  </ul>
  </div>
</div>

<div>
  <h4>Optical Flow</h4>
  <div>
  <ul style="list-style-type:circle;">
    <li>Superpixel-Based Large Displacement Optical Flow <a href="http://mml.citi.sinica.edu.tw/papers/SPLDOF_code.php">(Matlab)</a></li>
  </ul>
  </div>
</div>


<!-- [Grids] pages/sw.md -->
<div class="projects">
{%- if page.display_grids %}
  {%- if site.enable_project_categories and page.display_categories %}
    <!-- Display categorized projects -->
    {%- for category in page.display_categories %}
    <h2 class="category" style="text-align: left; color: #00369f">{{ category }}</h2>
    
    <!-- CY 01.24.21: new sw collection -->
    {%- assign categorized_projects = site.projects | where: "category", category -%}
    <!-- {%- assign categorized_projects = site.projects | where: "category", category -%} -->

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
    {%- assign sorted_projects = site.software | sort: "importance" -%}
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
