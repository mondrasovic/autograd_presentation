---
marp: true
theme: uncover
paginate: true
size: 16:9
title: Demystifying Automatic Differentiation
footer:	""
class:
    - invert

---

<style>
  h2 {
    font-size: 45px;
  }

  h3 {
    font-size: 40px;
  }

  .horizontal-section {
    display: flex;
  }

  .vertical-section {
    display: flex;
    flex-direction: column;
  }

  .important-term-horizontal {
    background-color: #151515; 
    color: #fff; 
    padding: 20px;
    border-radius: 10px;
    margin-right: 10px;
    margin-top: 10px;
    flex: 1;
    text-align: center;
  }

  .important-term-vertical {
    background-color: #151515; 
    color: #fff; 
    padding: 20px;
    border-radius: 10px;
    margin-bottom: 10px;
    flex: 1;
    text-align: center;
  }

  .advantage-section {
    background-color: #08a684;
    color: #fff; 
    padding: 10px;
    border-radius: 10px;
    margin-right: 10px;
    margin-top: 10px;
    flex: 1;
    text-align: center;
  }

  .disadvantage-section {
    background-color: #a83232;
    color: #fff; 
    padding: 10px;
    border-radius: 10px;
    margin-right: 10px;
    margin-top: 10px;
    flex: 1;
    text-align: center;
  }

  footer {
    color: #ccc;
  }
</style>

<!--
_header: ''
_footer: 📧 milan.ondrasovic@gmail.com | 📃 https://github.com/mondrasovic
_paginate: false
-->

# **Demystifying Automatic Differentiation**

## ***Linear Algebra Under the Hood***

<br>

***Milan Ondrašovič***

<span style="font-size:70%">**Machine learning research engineer** at [ROSSUM](https://rossum.ai) Czech Republic, s.r.o.</span>

---
<!--
header: Introduction - Prerequisite Knowledge
_footer: https://python.org | https://numpy.org
backgroundImage: linear-gradient(to top, #202228, #171717)
-->
## Prerequisites

![bg right:28% fit opacity:0.7](./images/numpy_logo.png)
![bg right:28% vertical fit opacity:0.7](./images/python_logo.png)

<div class="horizontal-section">
  <div class="important-term-horizontal">
    🐍
    <br>
    Python
  </div>

  <div class="important-term-horizontal">
    🔢
    <br>
    NumPy
  </div>

  <div class="important-term-horizontal">
    📝
    <br>
    Algebra
  </div>
</div>

---
## General Workflow

Choose an operation
Compute its derivative with respect to the input
Implement the derivative for backward pass

---
## Tensor - The Building Block

```Python
import numpy as np

class Tensor:
```

---
## Operation: Addition

---
## Backward
