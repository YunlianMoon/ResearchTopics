# Semantic

### Table of Contents
- Task
- Paper

### Task
Semantic represents the objects, layouts and any other semantic information describing the environment.

Given a target object class, *e.g. microwave*, the task is to navigate to an instance of an object from this class using only visual observations.

### paper

Visual semantic planning using deep successor representations \[2017, ICCV, Yuke Zhu\] \[[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Visual_Semantic_Planning_ICCV_2017_paper.pdf)\] \[[video](https://www.youtube.com/watch?v=_2pYVw6ATKo)\]<br/>
`algorithm:` IL + RL<br/>
`method:` (internal state(one-hot) --> FC + observation --> CNN + (action(one-hot) --> FC + action augment(one-hot) --> FC) --> FC) --> (state-action feature + successor feature + reward predictor) --> (reward + Q value)<br/>
`environment:` AI2-THOR

Visual semantic navigation using scene priors \[2019, ICLR, Wei Yang\] \[[paper](https://arxiv.org/pdf/1810.06543.pdf)\] \[[video](https://www.youtube.com/watch?v=otKjuO805dE&feature=youtu.be)\]<br/>
`method:` ((images --> ResNet50 --> FC) + (word --> fasttext --> FC) + (knowledge graph--> GCN --> FC)) --> FC --> policy (A3C)<br/>
`environment:` AI2-THOR

Learning to Learn How to Learn: Self-Adaptive Visual Navigation Using Meta-Learning \[2019, CVPR, Mitchell Wortsman\] \[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wortsman_Learning_to_Learn_How_to_Learn_Self-Adaptive_Visual_Navigation_Using_CVPR_2019_paper.pdf)\] \[[code](https://github.com/allenai/savn)\] \[[video](https://www.youtube.com/watch?v=-Ba6ZRMcxEE&feature=youtu.be)\]<br/>
`method:`<br/>
`environment:` AI2-THOR







