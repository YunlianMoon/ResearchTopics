# Visual Navigation using DRL

### Table of Contents
- Survey
- Paper
  - <a href="#image">image</a>
  - <a href="#VLN">vision and language</a>
    - <a href="#PG">point goal</a>
    - <a href="#OG">object goal</a>
    - <a href="#AG">area goal</a>
    - <a href="#instruction">instruction</a>
    - <a href="#question">question</a>

#### <a name="OG">object goal</a>

Visual semantic planning using deep successor representations \[2017, ICCV, Yuke Zhu\] \[[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Visual_Semantic_Planning_ICCV_2017_paper.pdf)\]<br/>
`method: image + action --> CNN --> successor representation (SR)`<br/>
`environment: AI2-THOR`

Visual representations for semantic target driven navigation \[2018, arxiv, Arsalan Mousavian\] \[[paper](https://arxiv.org/pdf/1805.06066.pdf)\]<br/>
`description: reward (distance)`<br/>
`method: ((image --> ResNet50) + target (one-hot) + action + success binary indicator (colison) + object detection + semantic segmentation + depth image) --> CNN --> LSTM --> NN --> policy (imitation learning + DQN)`<br/>
`environment: SUNCG, AVD`

Visual semantic navigation using scene priors \[2018, arxiv, Wei Yang\] \[[paper](https://arxiv.org/pdf/1810.06543.pdf)\]<br/>
`method: ((4 history images --> ResNet50) + (goal --> word embedding) + (graph knowledge --> GCN)) --> NN --> policy (A3C)`<br/>
`environment: AI2-THOR`

Understanding grounded language learning agents \[2017, arxiv, Felix Hill\] \[[paper](https://arxiv.org/pdf/1710.09867.pdf)\]<br/>
`method: ((image --> CNN) + (textual instruction) --> LSTM) --> NN --> LSTM --> policy (A3C)`<br/>
`environment: DeepMind Lab`

Zero-shot task generalization with multi-task deep reinforcement learning \[2017, ICML, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1706.05064.pdf)\]<br/>
`method: `<br/>
`environment: Minecraft`

Grounded language learning in a simulated 3d world \[2017, arxiv, Karl Moritz Hermann\] \[[paper](https://arxiv.org/pdf/1706.06551.pdf)\]<br/>
`method: ((image --> CNN) + (textual instruction --> LSTM)) --> NN --> LSTM --> policy (A3C) + autoencoder auxiliary task + language      prediction`<br/>
`environment: DeepMind Lab`

Gated-attention architectures for task-oriented language grounding \[2018, AAAI, Devendra Singh Chaplot\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/viewFile/17425/16578)\]<br/>
`description: unseen instructions/maps`<br/>
`method: ((image --> CNN) + (text instruction --> GRU)) --> attention --> NN --> LSTM --> NN --> policy (A3C) + imitation learning`<br/>
`environment: ViZDoom`

#### <a name="AG">area goal</a>

Building generalizable agents with a realistic and rich 3d environment \[2018, arxiv, Yi Wu\] \[[paper](https://arxiv.org/pdf/1801.02209.pdf?utm_content=buffer53a22&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)\]<br/>
`description: unseen environments`<br/>
`method: (((depth image + semantic segmentation + image) --> CNN) + (concept --> embedding)) --> NN --> LSTM --> policy (A3C/DDPG)`<br/>
`environment: House3D`

#### <a name="instruction">instruction</a>

Mapping instructions and visual observations to actions with reinforcement learning \[2017, arxiv, Dipendra Misra\] \[[paper](https://arxiv.org/pdf/1704.08795.pdf)\]<br/>
`method: ((image --> CNN) + (instruction --> LSTM) + (action --> NN)) --> NN --> policy (policy gradient)`<br/>
`environment: block world`

Vision-and-language navigation: Interpreting visually-grounded navigation instructions in real environments \[2018, CVPR, Peter Anderson\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Anderson_Vision-and-Language_Navigation_Interpreting_CVPR_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: ((instruction --> LSTM) + (image --> ResNet152) + (action --> NN)) --> attention --> LSTM --> imitation learning`<br/>
`environment: R2R`

Look before you leap: Bridging model-free and model-based reinforcement learning for planned-ahead vision-and-language navigation \[2018, ECCV, Xin Wang\] \[[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xin_Wang_Look_Before_You_ECCV_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: model-free + model-based`<br/>
`environment: R2R`

Speaker-follower models for vision-and-language navigation \[2018, NIPS, Daniel Fried\] \[[paper](https://papers.nips.cc/paper/7592-speaker-follower-models-for-vision-and-language-navigation.pdf)\]<br/>
`description: unseen environment`<br/>
`method: fllower module + speaker module`<br/>
`environment: R2R`

Reinforced Cross-Modal Matching and Self-Supervised Imitation Learning for Vision-Language Navigation \[2018, arxiv, Xin Wang\] \[[paper](https://arxiv.org/pdf/1811.10092.pdf)\]<br/>
`description: unseen environments`<br/>
`method: (textual instruction --> NN + (images --> CNN --> attention + action) --> LSTM) --> attention --> policy (imitation learning + A3C)`<br/>
`environment: R2R`

#### <a name="question">question</a>

Iqa: Visual question answering in interactive environments \[2018, CVPR, Daniel Gordon\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Gordon_IQA_Visual_Question_CVPR_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: navigator + manipulator + detector + scanner + answerer`<br/>
`method: (((image --> CNN) + action) --> GRU + question --> LSTM + semantic memory --> NN) --> NN --> policy (A3C)`<br/>
`environment: AI2-THOR`

Embodied question answering \[2018, CVPR, Abhishek Das\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Das_Embodied_Question_Answering_CVPR_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: hierarchical model`<br/>
`method: (image --> CNN + question --> LSTM) --> NN or LSTM --> policy (REINFORCE)`<br/>
`environment: House3D`






