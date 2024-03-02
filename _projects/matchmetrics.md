---
layout: page
title: Soccer Analytics
description: Combining two passions
img: assets/img/soccer-ball.jpeg
importance: 4
category: work
---

I've enjoyed playing and watching soccer since I was a little kid. Starting with my <a href='/assets/pdf/bachelor-thesis.pdf'>BSc thesis</a>, I was able to combine this pashion with my interest in data science. I developed a model for predicting the outcomes of Premier League games, finding that financial features are as informative as performance-based metrics.

During my master's degree, I joined a local startup called <a href="https://matchmetrics.com">matchmetrics</a> and developed models for <a href="https://web.archive.org/web/20240204175435/https://matchmetrics.com/insights/how-can-i-compare-players-across-competitions-and-countries/">predicting player performance across different leagues and countries</a>.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/matchmetrics-competition-level.jpg" title="competition levels" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    ©matchmetrics GmbH. Ratings and stability of different European competitions.
</div>

My work culminated in my <a href='/assets/pdf/master-thesis.pdf'>MSc thesis</a>, where I developed a model to predict events in the video feed of a soccer game. The model was able to detect events such as passes, crosses, dribblings, and shots with high accuracy.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="/assets/video/msc-video.webm" class="img-fluid rounded z-depth-1" controls=true %}
    </div>
</div>
<div class="caption">
    The inner green/red border indicates a ground truth event. The outer border indicates a predicted event. The model is correct when both the inner and outer borders are the same color.
</div>