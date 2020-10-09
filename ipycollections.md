---
title: ipycollections
layout: single
sidebar:
  - title: "ipycollections"
    image: assets/images/ipycollections-icon.svg
    links:
      - label: "GitHub"
        icon: "fab fa-fw fa-github"
        url: "https://github.com/dataflownb/ipycollections-extension"
      - label: "PyPI"
        icon: "fab fa-fw fa-python"
        url: "https://pypi.org/project/ipycollections/"
      - label: "npm"
        icon: "fab fa-fw fa-npm"
        url: "https://www.npmjs.com/package/@dfnotebook/ipycollections-extension"
---

ipycollections provides users more control over the detail of each output shown while preserving rich displays in collections. Like other tools and Jupyter's own JSON renderer, collections like lists and dictionaries can be summarized and truncated while allowing users to view more data. At the same time, outputs that are nested inside of these collections can now be richly displayed. Thus, we can have a list of images or dataframes displayed in a more meaningful format.

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/ipycollections-before.svg" alt="">
  <figcaption>Standard Jupyter/IPython Output</figcaption>
</figure> 

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/ipycollections-after.svg" alt="">
  <figcaption>ipycollections Output</figcaption>
</figure>

ipycollections consists of both an IPython extension that addds a new formatter to process collections into a JSON serialization, and a JupyterLab plugin that renders the JSON serialization into output that can be collapsed and expanded. The plugin delegates rendering of rich outputs to their respective renderers.

{% include video id="YgJ8HDRXCy8" provider="youtube" %}
