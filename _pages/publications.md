---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed publications and manuscripts under review.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h2 class="bibliography">first-author publications</h2>

{% bibliography --group_by none --query @*[authorship=first]* %}

<h2 class="bibliography">co-authored publications</h2>

{% bibliography --group_by none --query @*[authorship=co]* %}

<h2 class="bibliography">manuscripts under review</h2>

<!-- Same markup as the gem's bib.liquid so these match the entries above and work with the search box. -->
<ol class="bibliography">
  <li>
    <div class="row">
      <div class="col col-sm-2 abbr"><abbr class="badge rounded w-100">Under review</abbr></div>
      <div class="col-sm-8">
        <div class="title">ReVisiT: Revisiting Only What Changed for Efficient Video Vision Transformers</div>
        <div class="periodical">
          Training-free selective inference that recomputes only the tokens that changed between frames and reuses cached activations elsewhere.
        </div>
        <div class="links">
          <a href="{{ '/projects/revisit/' | relative_url }}" class="btn btn-sm z-depth-0" role="button">Project</a>
        </div>
      </div>
    </div>
  </li>
  <li>
    <div class="row">
      <div class="col col-sm-2 abbr"><abbr class="badge rounded w-100">Under review</abbr></div>
      <div class="col-sm-8">
        <div class="title">What a Late Condition Misses: Correcting Mid-Trajectory Condition Changes</div>
        <div class="periodical">
          Missed-Guidance Correction (MGC), a training-free method that adapts diffusion and flow samplers to conditions that arrive mid-generation.
        </div>
        <div class="links">
          <a href="{{ '/projects/mgc/' | relative_url }}" class="btn btn-sm z-depth-0" role="button">Project</a>
        </div>
      </div>
    </div>
  </li>
  <li>
    <div class="row">
      <div class="col col-sm-2 abbr"><abbr class="badge rounded w-100">Under review</abbr></div>
      <div class="col-sm-8">
        <div class="title">SCENE: A Sparse Capacitive Event-Driven Near-Sensor Engine for Frame-Compatible Object Detection</div>
        <div class="periodical">Reconstructs conventional video frames from sparse updates so existing object detectors can process them.</div>
        <div class="links">
          <a href="{{ '/projects/scene/' | relative_url }}" class="btn btn-sm z-depth-0" role="button">Project</a>
        </div>
      </div>
    </div>
  </li>
</ol>

</div>
