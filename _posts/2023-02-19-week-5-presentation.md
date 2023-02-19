---
layout: post
author: Karl
title: Week 5 Update
brief: Building the comments pipeline.
---

# Week 5 Progress Report

[Progress Report Presentation]({{site.url}}/assets/pptx/presentation-week-05.pptx)

[Progress Report PDF]({{site.url}}/assets/pdfs/progress-week-05.pdf)

## Integration Test

We documented an integration test performed on 2/18/2023. In the 5 minute video, I describe the bugs we encountered and how we fixed them to have a succesful integration test.

{% include video.html content="2022-02-18-Integrationtest-1.mp4" %}

## Devlog Videos

This week, I also created a few extra videos documenting my coding process. There is no narration, only music and 4000% speed coding.

### ExtractPath video

The first video is the implementation of "ExtractPath" which extracts a domain and sub-path from a url string. I struggled with Golangs regex library for a little while, but I got it in the end.

{% include video.html content="2022-02-17-Extractpathregex.mp4" %}

### Initialize Page, Get Comments video

The second video is code to initialize a Page object and populate it with comments from the database. I had to think about how to transform database rows into Server-Client communication entities.

{% include video.html content="2022-02-17-Initializepage.mp4" %}

### New Comments video

The third video is the implementation of the newComment pipeline, which allows a user to post a new comment.

{% include video.html content="2022-02-18-Newcomment-30wsSpr.mp4" %}



