# Visual Navigation using DRL

### Table of Contents
- Paper
  - <a href="#image">image</a>
    - <a href="#same">same envirionment/task for evaluation</a>
    - <a href="#unseen">generalization</a>
  - <a href="https://github.com/YunlianMoon/ResearchTopics/blob/master/VisualNavigation/vision_and_language.md">vision and language</a>

### Paper

#### <a name="image">image</a>

#### <a name="same">same environment/task</a>

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\]<br/>
`method: image --> CNN --> successor representation (SR)`<br/>
`environment: MazeBase gridworld, VizDoom`

A deep hierarchical approach to lifelong learning in minecraft \[2017, AAAI, Chen Tessler\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14630/13950)\]<br/>
`method: image --> (CNN --> Q) + (CNN --> skills) --> policy (DQN)`<br/>
`environment: Minecraft`

Learning to navigate in complex environments \[2016, arxiv, Piotr Mirowski\] \[[paper](https://arxiv.org/pdf/1611.03673.pdf)\]<br/>
`method: (image --> CNN) + additional inputs (velocity, action, reward) --> stacked LSTM --> policy (A3C) + auxiliary losses (depth prediction, loop closure detection)`<br/>
`environment: DeepMind Lab`

Reinforcement learning with unsupervised auxiliary tasks \[2016, arxiv, Max Jaderberg\] \[[paper](https://arxiv.org/pdf/1611.05397.pdf)\] \[[code](https://github.com/miyosuda/unreal)\]<br/>
`method: (image --> CNN + action + reward) --> LSTM --> policy (A3C) + auxiliary losses`<br/>
`environment: Labyrinth`

Training agent for first-person shooter game with actor-critic curriculum learning \[2017, ICLR, Yuxin Wu\] \[[paper](https://openreview.net/pdf?id=Hk3mPK5gg)\]

Deepnav: Learning to navigate large cities \[2017, CVPR, Samarth Brahmbhatt\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Brahmbhatt_DeepNav_Learning_to_CVPR_2017_paper.pdf)\] \[[code](https://github.com/samarth-robo/deepnav_cvpr17)\]<br/>
`method: supervised learning`<br/>
`environment: Google Street View`

A deep Q network for robotic planning from image \[2017, ICARM, Jianhui Han\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8273235)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: Gazebo`

Application of deep reinforcement learning in mobile robot path planning \[2017, CAC, Jing Xin\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8244061)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: DeepMind Lab`

One-shot reinforcement learning for robot navigation with interactive replay \[2017, arxiv, Jake Bruce\] \[[paper](https://arxiv.org/pdf/1711.10137.pdf)\]

Self-supervised deep reinforcement learning with generalized computation graphs for robot navigation \[2018, ICRA, Gregory Kahn\] \[[paper](https://arxiv.org/pdf/1709.10489.pdf)\]

#### <a name="unseen">generalization</a>

Control of memory, active perception, and action in minecraft \[2016, arxiv, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1605.09128.pdf)\] \[[code](https://github.com/junhyukoh/icml2016-minecraft)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (DQN)`<br/>
`environment: Minecraft`

Target-driven visual navigation in indoor scenes using deep reinforcement learning \[2017, ICRA, Yuke Zhu\] \[[paper](https://arxiv.org/pdf/1609.05143.pdf,)\] \[[code](https://github.com/yushu-liu/icra2017-visual-navigation)\]<br/>
`method: (image + target image) --> ResNet50 --> generic siamese layers --> scene-specific layers: policy (A3C)`<br/>
`environment: AI2-THOR`

Transfer deep reinforcement learning in 3d environments: An empirical study \[2016, NIPS, Devendra Singh Chaplot\] \[[paper](http://www.cs.cmu.edu/~rsalakhu/papers/DeepRL_Transfer.pdf)\]<br/>
`method: image --> CNN --> policy: DQN`<br/>
`environment: VizDoom`

Neural map: Structured memory for deep reinforcement learning \[2017, arxiv, Emilio Parisotto\] \[[paper](https://arxiv.org/pdf/1702.08360.pdf)\]<br/>
`method: image --> CNN --> LSIM --> Memory --> policy (A3C)`<br/>
`environment: 2D maze, VizDoom`

Learning to navigate in cities without a map \[2018, NIPS, Piotr Mirowski\] \[[paper](https://papers.nips.cc/paper/7509-learning-to-navigate-in-cities-without-a-map.pdf)\] \[[code](https://github.com/deepmind/streetlearn)\]<br/>
`method: (image --> CNN) + (goal description, reward, action) --> LSTM --> policy (A3C) + auxiliary losses`<br/>
`environment: Google Street View`

Zero-shot visual imitation \[2018, CVPR, Deepak Pathak\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Pathak_Zero-Shot_Visual_Imitation_CVPR_2018_paper.pdf)\] \[[code](https://github.com/pathak22/zeroshot-imitation)\]<br/>
`method: ((image + goal image) --> CNN) + action --> LSTM --> policy (imitation learing) + auxiliary losses`<br/>
`environment: VizDoom`

Unsupervised predictive memory in a goal-directed agent \[2018, arxiv, Greg Wayne\] \[[paper](https://arxiv.org/pdf/1803.10760.pdf)\] \[[code](https://github.com/yosider/merlin)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (A3C)`<br/>
`environment: DeepMind Lab`
