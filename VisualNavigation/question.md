# Question

### Table of Contents
- <a href="#task">Task</a>
- <a href="#webcite">Webcite</a>
- <a href="#paper">Paper</a>

### <a name="task">Task</a>
An agent is spawned at a random location in a 3D environment and asked a question. In order to answer, the agent must first intelligently navigate to explore the environment, gather necessary visual information through first-person (egocentric) vision, and then answer the question.

### <a name="webcite">Webcite</a>

[Embodied Question Answering](https://embodiedqa.org/)

### <a name="paper">Paper</a>

Iqa: Visual question answering in interactive environments \[2018, CVPR, Daniel Gordon\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Gordon_IQA_Visual_Question_CVPR_2018_paper.pdf)\] \[[code](https://github.com/danielgordon10/thor-iqa-cvpr-2018)\] \[[video](https://www.youtube.com/watch?v=pXd3C-1jr98&feature=youtu.be)\]<br/>
`description:` unseen environments<br/>
`idea:` navigator + manipulator + detector + scanner + answerer<br/>
`method:` (((image --> CNN) + action) --> GRU + question --> LSTM + semantic memory --> CNN) --> FC --> policy (A3C)<br/>
`environment:` AI2-THOR

Embodied question answering \[2018, CVPR, Abhishek Das\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Das_Embodied_Question_Answering_CVPR_2018_paper.pdf)\] \[[code](https://github.com/facebookresearch/EmbodiedQA)\] \[[video](https://www.youtube.com/watch?v=gVj-TeIJfrk)\]<br/>
`description:` unseen environments<br/>
`idea:` hierarchical model<br/>
`method:` (image --> CNN + question --> LSTM) --> NN or LSTM --> policy (REINFORCE)<br/>
`environment:` House3D

Embodied Question Answering in Photorealistic Environments with Point Cloud Perception \[2019, CVPR, Erik Wijmans\] \[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wijmans_Embodied_Question_Answering_in_Photorealistic_Environments_With_Point_Cloud_Perception_CVPR_2019_paper.pdf)\]<br/>
`observation representations:` RGB, RGB-D, semantic segmentation, color autoencoding, structure autoencoding, depth prediction<br/>
`idea:` Inflection Weighting, weight predictions at time steps more heavily if the ground truth action differs from the previous one<br/>
`method:` (image --> ResNet50 + question --> LSTM) --> imitation learning<br/>
`environment:` Matterport 3D

Multi-target embodied question answering \[2019, CVPR, Licheng Yu\] \[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yu_Multi-Target_Embodied_Question_Answering_CVPR_2019_paper.pdf)\] \[[video](https://www.youtube.com/watch?v=pK5gYk9OgjE)\]<br/>
`method:` program generator, controller, navigator, VQA<br/>
`environment:` House3D







