---
title: Classical Machine learning in Image Processing
layout: single
author: Laura Boucheron
author_profile: true
header:
  overlay_color: "444444"
  overlay_image: /assets/images/margaret-weir-GZyjbLNOaFg-unsplash_dark.jpg
---

**Last Update:** 3 May 2021 <br /> **RMarkdown:**

## Overview

In this tutorial, we present a brief overview of classical machine learning concepts as applicable to image classification applications. In this tutorial, we will develop a classical machine learning algorithm capable of discriminating between objects present in an image. This walk through was originally written in python: [link to python version](). We have tried to maintain functionality across both languages but certain libraries/features may only be available in one or the other. The basics concepts should be the same across both.

This tutorial explores:

-
-
-

## Section 1: Working with the CalTech101 Dataset

### Exploring the Images

In the previous tutorial, we were working with only two images. There are more than 8000 images in 101 different directories in the CalTech101 dataset. We thus need to develop ways to efficiently loop over larger image datasets and access the images without hard coding the image filenames.

```
 categories=sort(list.files(full.names = TRUE,"101_objectCategories"))
```
