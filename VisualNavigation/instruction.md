# Instruction

### Table of Contents
- Task
- Paper
  - <a href="#short">short instruction</a>
  - <a href="#long">long instruction</a>

### Task
An agent directly maps raw visual observations and text input to actions for instruction execution.

### Paper

#### <a name="short">short instruction</a>

Zero-shot task generalization with multi-task deep reinforcement learning \[2017, ICML, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1706.05064.pdf)\] \[[video](https://sites.google.com/a/umich.edu/junhyuk-oh/task-generalization)\] \[[webcite](https://sites.google.com/a/umich.edu/junhyuk-oh/task-generalization)\]<br/>
`method:` (((instructions + image) --> meta controller (CNN + LSTM)) + image) --> paremetrirized sill (CNN + LSTM) --> policy (A2C) + termination prediction<br/>
`environment:` Minecraft

Gated-attention architectures for task-oriented language grounding \[2018, AAAI, Devendra Singh Chaplot\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/viewFile/17425/16578)\] \[[code](https://github.com/devendrachaplot/DeepRL-Grounding)\] \[[video](https://github.com/devendrachaplot/DeepRL-Grounding)\] \[[webcite](https://sites.google.com/view/gated-attention/home)\]<br/>
`description:` unseen instructions/maps<br/>
`method:` ((image --> CNN) + (text instruction --> GRU --> FC --> attention vector)) --> FC --> LSTM --> (policy (A3C) + imitation learning (behavioral cloning/DAgger))<br/>
`environment:` ViZDoom

Grounded language learning in a simulated 3d world \[2017, arxiv, Karl Moritz Hermann\] \[[paper](https://arxiv.org/pdf/1706.06551.pdf)\] \[[code](https://github.com/dai-dao/Grounded-Language-Learning-in-Pytorch)\] \[[video](https://www.youtube.com/watch?v=wJjdu1bPJ04&feature=youtu.be)\]<br/>
`method:` ((image --> CNN) + (textual instruction --> LSTM)) --> NN --> LSTM --> (policy (A3C) + autoencoder auxiliary task + language      prediction)<br/>
`environment:` DeepMind Lab

Understanding grounded language learning agents \[2017, arxiv, Felix Hill\] \[[paper](https://arxiv.org/pdf/1710.09867.pdf)\] \[[video](https://www.youtube.com/watch?v=9vY8D4wuEV0)\]<br/>
`method:` ((image --> CNN) + (textual instruction) --> LSTM) --> FC --> LSTM --> policy (A3C)<br/>
`environment:` DeepMind Lab

Building generalizable agents with a realistic and rich 3d environment \[2018, ICLR, Yi Wu\] \[[paper](https://arxiv.org/pdf/1801.02209.pdf?utm_content=buffer53a22&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)\]<br/>
`description:` unseen environments<br/>
`method:` (((depth image + semantic segmentation + image) --> CNN) + (concept --> embedding)) --> NN --> LSTM --> policy (A3C/DDPG)<br/>
`environment:` House3D

#### <a name="long">long instruction</a>

Mapping instructions and visual observations to actions with reinforcement learning \[2017, arxiv, Dipendra Misra\] \[[paper](https://arxiv.org/pdf/1704.08795.pdf)\] \[[code](https://github.com/lil-lab/blocks)\]<br/>
`method:` ((image --> CNN) + (instruction --> LSTM) + (action --> NN)) --> NN --> policy (policy gradient)<br/>
`environment:` block world

Vision-and-language navigation: Interpreting visually-grounded navigation instructions in real environments \[2018, CVPR, Peter Anderson\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Anderson_Vision-and-Language_Navigation_Interpreting_CVPR_2018_paper.pdf)\]<br/>
`description:` unseen environments<br/>
`method:` ((instruction --> LSTM) + ((image --> ResNet152 + action) --> LSTM)) --> attention --> teacher-forcing/student-forcing<br/>
`environment:` R2R

Scheduled policy optimization for natural language communication with intelligent agents \[2018, arxiv, Wenhan Xiong\] \[[Paper](https://arxiv.org/pdf/1806.06187.pdf)\]<br/>
`mehtod:` (image --> CNN + instruction --> LSTM + action --> NN) --> policy (imitation learning + PPO/REINFORCE/A2C/DQN)<br/>
`environment:` block-world

Look before you leap: Bridging model-free and model-based reinforcement learning for planned-ahead vision-and-language navigation \[2018, ECCV, Xin Wang\] \[[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xin_Wang_Look_Before_You_ECCV_2018_paper.pdf)\]<br/>
`description:` unseen environments<br/>
`method:` model-free + model-based<br/>
`method:` ((image --> CNN) + (instruction --> attention --> LSTM) ) --> LSTM --> policy (REINFORCE)<br/>
`environment:` R2R

Reinforced Cross-Modal Matching and Self-Supervised Imitation Learning for Vision-Language Navigation \[2018, arxiv, Xin Wang\] \[[paper](https://arxiv.org/pdf/1811.10092.pdf)\]<br/>
`description:` unseen environments<br/>
`reward:` Extrinsic Reward (relative navigation distance/success) + Intrinsic Reward (instruction reconstruction)<br/>
`method:` (textual instruction --> LSTM + (images --> ResNet152 --> attention + action) --> LSTM) --> attention --> policy (imitation learning + REINFORCE)<br/>
`environment:` R2R
