---
layout: page
title: KickStarter Novelty Detection
description: A classifier that can classify function of images in Kickstarter projects
img: /assets/img/project_kickstarter/kickstarter_header.png
importance: 1
category: 
status: ongoing
keywords: [data science, kickstarter, image]
---
<style>
  body {
  text-align: justify}
  </style>
<h4><strong>Brief Introduction</strong></h4>
Kickstarter novelty detection is an on-going project. We aimed at designing a comprehensive score to scale the novelty level in projects and linking the novelty score with the successfullness of the project.

<h4><strong>Plan of Work</strong></h4>
The work is divided to two stages.

<strong>Stage 1: Image Classifier [Current]</strong>

we want to create a image classifier that can distinguish the functions of images in the project descriptions.

<strong>[Our Motivation]</strong>

We noticed that images in descriptions of the projects must be there for some reason. Therefore, we divide the images into 10 categories based on the purpose of images. We hope that with the created Image Classifier, further research would easily classify the purpose of images in the descriptions without human labelling.

<strong>[Difficulties]</strong>

<div>
    <li>
        [Lack of Data] - Even though we scrape images from thousands of projects, the number of images in some categories is still not enough.
    </li>
    <li>
        [Unbalanced Data] - Some categories have way more samples than others.
    </li>
    <li>
        [Poor Performance] - The baseline auc is only around .5, which means that the model learns nothing.
    </li>
</div>


<strong>Stage 2: Comprehensive Score</strong>

<h4>This is still an working paper, Stay tuned!</h4>