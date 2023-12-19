Deep Feature Flow is initially described in a CVPR 2017 paper. It provides a simple, fast, accurate, and end-to-end framework for video recognition (e.g., object detection and semantic segmentation in videos). It is worth noting that:

<img width="454" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/81f7dd4e-9848-44ca-abf5-147ea3f9153e">
<img width="398" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/419d62b2-8feb-46e6-b199-c0506a0d4342">


Deep Feature Flow significantly speeds up video recognition by applying the heavy-weight image recognition network (e.g., ResNet-101) on sparse key frames, and propagating the recognition outputs (feature maps) to the other frames by the light-weight flow network (e.g., FlowNet).
The entire system is end-to-end trained for the task of video recognition, which is vital for improving the recognition accuracy. Directly adopting state-of-the-art flow estimation methods without end-to-end training would deliver noticable worse results.
Deep Feature Flow can easily make use of sparsely annotated video recognition datasets, where only a small portion of the frames are annotated with ground-truth labels.
Click image to watch our demo video

Demo Video on YouTube Demo Video on YouTube
