---
layout: page
title: Image Processing on FPGAs using PYNQ (PYNQ Z2 board)
# description: a project with a background image
img: assets/img/12.jpg
importance: 1
category: FPGA
related_publications: true
---

Will update more details when having more time

This project is instructed under professor [Le,Binh](https://www.sjsu.edu/people/binh.q.le/)

Based on: [Accelerating Image Processing on FPGAs using HLS and PYNQ](https://ieeexplore.ieee.org/document/9277085)

- Perform Conv-based techniques on a given input image.
- Initially store the image in DDR through an external interface.
- Configure the DMA controoler (axi_dma) to stream the image data from the user IP.
- The stream IP processes the image one or more pixel at a time and streams back the processed data to the DMA Controller
DMA controller receives the stream data from the IP and sends it back to the external DDR memory through AXI4 interface.
- Processed image is sent back in the memory which can be sent to external world using interfaces or display controllers.
