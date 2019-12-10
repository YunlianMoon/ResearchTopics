# question

### Table of Contents
- Task
- Paper

### Task
An agent is spawned at a random location in a 3D environment and asked a question. In order to answer, the agent must first intelligently navigate to explore the environment, gather necessary visual information through first-person (egocentric) vision, and then answer the question.

### Paper

Iqa: Visual question answering in interactive environments \[2018, CVPR, Daniel Gordon\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Gordon_IQA_Visual_Question_CVPR_2018_paper.pdf)\] \[[code](https://github.com/danielgordon10/thor-iqa-cvpr-2018)\] \[[video](https://www.youtube.com/watch?v=pXd3C-1jr98&feature=youtu.be)]<br/>
`description:` unseen environments<br/>
`idea:` navigator + manipulator + detector + scanner + answerer<br/>
`method:` (((image --> CNN) + action) --> GRU + question --> LSTM + semantic memory --> CNN) --> FC --> policy (A3C)<br/>
`environment:` AI2-THOR

Embodied question answering \[2018, CVPR, Abhishek Das\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Das_Embodied_Question_Answering_CVPR_2018_paper.pdf)\] \[[code](https://github.com/facebookresearch/EmbodiedQA)\]<br/>
`description: unseen environments`<br/>
`method: hierarchical model`<br/>
`method: (image --> CNN + question --> LSTM) --> NN or LSTM --> policy (REINFORCE)`<br/>
`environment: House3D`
