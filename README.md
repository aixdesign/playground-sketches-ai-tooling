# AI Tooling: playground-sketches-to-images

Experiment on creating an image segmentation model to make playground sketches

Read the full log of my experiment [here](https://www.notion.so/nadiapiet/Experiment-2-Image-Segmentation-Playgrounds-from-sketches-Image-Segmentation-0c313cb9f4a34dbe84af57ac557ccf00). Very detailed description and log, including images and videos, of what I got up to.

![Image of a gauGAN](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1798d988-7536-41b7-992b-5782384a7ff6/gauGAN2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221222%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221222T133747Z&X-Amz-Expires=86400&X-Amz-Signature=7cf317134a3eb0c7bbe47b107aa46d4e9dd489e482283b1f4a5937be099e53fc&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22gauGAN2.png%22&x-id=GetObject)
<sup>Output from NVIDIA’s GauGAN2. Left is my sketch input with different colours, right is the output</sup>

If you prefer to watch over reading, I have [Part 1](https://www.instagram.com/p/CjA_zyqgdXB/) and [Part 2](https://www.instagram.com/p/CjDSVlYA7AR/) of my experiment process.

This is my version of code. Almost all I didn't write myself, so here's the references:

** Original [SPADE-COCO](https://github.com/agermanidis/SPADE-COCO) Github repo by agermanidis **

For dataset preparation I used:
- [COCO-Annotator](https://github.com/jsbroks/coco-annotator) is from jsbrooks. Docker was too difficult to set up so I abandoned this repo and went to...

- [labelme](https://github.com/wkentaro/labelme) is from wkentaro. 


For starting my synthetic dataset:

- playground_dataset folder has the blender files and scripts that I took from this tutorial by [Immersive Limit 'Synthetic Datasets With Blender'](https://www.immersivelimit.com/tutorials/synthetic-datasets-with-blender).
