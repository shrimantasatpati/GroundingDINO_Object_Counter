## GroundingDINO_Object_Counter
* Counting number of occurrences of several objects in single/multiple images
* Extending the GroundingDINO usability for counting and returning the total items detected

'''
- **CLASSES:** ['headlamp', 'men underwear', 'book', 'candy', 'paper', 'box', 'bottle'] #Classes to detect in images
  * Change the items of the CLASSES list to detect other objects
    
- **BOX_TRESHOLD:** 0.30
- **TEXT_TRESHOLD:** 0.20
'''

### Output images

1. **Object Counting On Single Image (Sample):**
   <p align="center">
   <img src="Output_images/Output_1.png" width=750></p>
  
##### Results for 20231121_121427.jpg: 
- headlamp: 3
- men underwear: 0
- book: 0
- candy: 0
- paper: 3
- box: 11
- bottle: 4

### Pro Tip: Use GPU Acceleration - Google Colab T4 GPU

## Steps in this Tutorial

In this tutorial, we are going to cover:

- **Before you start** - Make sure you have access to the GPU
- **Install Grounding DINO** - Setup Python environment.
- **Mount Example Data from Google Drive**
- **Load model**
- **Single Image Inference**
- **Multiple Image Inference**
---
### Dataset Link - Request to author
Credits - Inspired from [RoboFlow](https://github.com/roboflow/notebooks/tree/main/notebooks) GroundingDINO notebooks
- Research articles
   * [GroundingDINO Paper](https://arxiv.org/abs/2303.05499)
   * [Exaplanations](https://www.ikomia.ai/blog/grounding-dino-zero-shot-detection-explained)

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/IDEA-Research/GroundingDINO) [![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499)

Grounding DINO can detect **arbitrary objects** with human inputs such as category names or referring expressions. The key solution of open-set object detection is introducing language to a closed-set detector DINO. for open-set concept generalization. If you want to learn more visit official GitHub [repository](https://github.com/IDEA-Research/GroundingDINO) and read the [paper](https://arxiv.org/abs/2303.05499).

![grounding dino figure](https://media.roboflow.com/notebooks/examples/grounding-dino-figure.png)

