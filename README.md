<img width="981" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/e90f6d52-6fa1-4737-bde8-ac988851f14b">

REO(Resource efficient object detection) is initially described in a 2023 paper. It provides a simple, fast, accurate, and end-to-end framework for video object detection It is worth noting that:


The result is the following : 
<img width="454" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/81f7dd4e-9848-44ca-abf5-147ea3f9153e">
<img width="398" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/419d62b2-8feb-46e6-b199-c0506a0d4342">

REO significantly speeds up video recognition by applying the heavy-weight image recognition network (e.g., ResNet-101) on sparse key frames, and propagating the recognition outputs (feature maps) to the other frames by the light-weight flow network (e.g., Shallow Ver. ResNet-101).

The entire system is end-to-end trained for the task of video recognition, which is vital for improving the recognition accuracy. Directly adopting state-of-the-art flow estimation methods without end-to-end training would deliver noticable worse results.

REO can easily make use of sparsely annotated video recognition datasets, where only a small portion of the frames are annotated with ground-truth labels.

<img width="816" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/14885bf6-e422-45c4-86c3-e9e2b1e93c6a">

<img width="636" alt="image" src="https://github.com/HY-AI2-Projects/REO/assets/62403440/7e57d46e-f3c9-4b3c-8a19-392d89096180">

