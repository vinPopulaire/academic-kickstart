+++
title = "B.Sc Thesis: Fast object detection on images"
date = 2015-08-21T14:17:52+03:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["image processing", "object detection"]

# Project summary to display on homepage.
summary = """
Proposal of a new method for the extraction of object proposals on images, called Segment Boxes. This method uses segmentation of the image and by using the resulting segments, we score windows inside the image based on the possibility that they contain objects. We try to encapsulate good ideas of other methods as well as some of our own to achieve best results, so we end up with several approaches of our method.
"""

# Optional image to display on homepage.
image_preview = ""

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Does the project detail page use source code highlighting?
highlight = true

# URLs
url_pdf = "/files/theses/diplomatiki.pdf"
url_code = "https://github.com/vinPopulaire/ObjectProposals"
url_cite = ""

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++

Object proposals is a relatively new problem which appeared due to the complexity of modern object detectors and their high execution time. The purpose of object proposal algorithms is the high speed class-agnostic detection of all objects in the image. The proposals are then passed to the object detectors so that they avoid the exhaustive search of the image using the sliding window approach. This way, the time needed to detect objects is drastically reduced which enables them to use more complex and effective algorithms. Modern object detectors use object proposals.

In our thesis we present most modern methods for the extraction of object proposals and we propose a new method, Segment Boxes. This method uses segmentation of the image and by using the resulting segments we score windows inside the image based on the possibility that they contain objects. We try to encapsulate good ideas of other methods as well as some of our own to achieve best results, so we end up with several approaches of our method.

We compare those different approaches and the best ones are compared with the state-of-the-art methods, using the appropriate metrics, on images from datasets PASCAL VOC07 and ImageNet2013. We then use our proposals with a modern object detector which uses deep learning and convolutional neural networks, Fast R-CNN, and we compare again our results with those of other methods, this time on the problem of object detection.

Our goal was to examine the potential of segmentation on the problem of object proposals. The results of our method are competitive and in some cases exceed those of the state-of-the-art methods, while achieving low execution time (one of our approaches runs on 0.3 seconds per image).
