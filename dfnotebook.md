---
title: dfnotebook
layout: single
sidebar:
  - title: "dfnotebook"
    image: assets/images/dfnotebook-icon.svg
    links:
      - label: "GitHub"
        icon: "fab fa-fw fa-github"
        url: "https://github.com/dataflownb/dfnotebook-extension"
---

Dataflow notebooks are Jupyter notebooks written in Python that elevate outputs to serve as memorable links between cells. Instead of having to search and recall which cells contain variable definitions or mutations, all variables that are accessible in other cells are outputs and must be written (either as an expression or assignment) at the end of a cell. Because it does make sense to reuse variable names, each name refers to the *most recent* output, but older outputs can be referred to via scoped expressions (e.g. `df$full`).  

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/dfnotebook.svg" alt="">
  <figcaption>Dataflow Notebook</figcaption>
</figure> 

These notebooks are created using a modified JupyterLab notebook extension (dfnotebook-extension) and a modified IPython kernel (dfkernel). The notebook extension provides support for displaying named outputs, naming cells, and transforming referenced outputs to persistent identifiers. The kernel does more of the heavy lifting, recursively updating cells, parsing scoped expressions, and supporting completions. We are working on porting user interface elements to JupyterLab.

{% include video id="FvSL407aLqs" provider="youtube" %}
