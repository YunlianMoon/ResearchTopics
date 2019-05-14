# Visual Navigation using DRL

### Table of Contents
- Survey
- Paper
  - <a href="#image">image</a>
    - <a href="#same">same envirionment/task for evaluation</a>
    - <a href="#unseen">generalization</a>
  - <a href="#VLN">vision and language</a>
    - <a href="#PG">point goal</a>
    - <a href="#OB">object goal</a>
    - <a href="#AG">area goal</a>
    - <a href="#instrction">instruction</a>
    - <a href="#question">question</a>

### Survey

[Dhiman, Vikas, et al. "A critical investigation of deep reinforcement learning for navigation." arXiv preprint arXiv:1802.02274 (2018).](https://arxiv.org/pdf/1802.02274.pdf)

### Paper

#### <a name="image">image</a>

#### <a name="same">same environment/task</a>

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\]<br/>
`method: image --> CNN --> successor representation (SR)`<br/>
`environment: MazeBase gridworld, VizDoom`

A deep hierarchical approach to lifelong learning in minecraft \[2017, AAAI, Chen Tessler\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14630/13950)\]<br/>
`method: image --> (CNN --> Q) + (CNN --> skills) --> policy (DQN)`
`environment: Minecraft`

A robot exploration strategy based on q-learning network \[2016, RCAR, Tai Lei\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7784001)\]

Towards cognitive exploration through deep reinforcement learning for mobile robots \[2016, arxiv, Lei Tai\] \[[paper](https://arxiv.org/pdf/1610.01733.pdf)\]

Deep reinforcement learning in a 3-d blockworld environment \[2016, IJCAI, Trevor Barron\] \[[paper](http://cs.coloradocollege.edu/~mwhitehead/files/mypapers/blockworld.pdf)\]<br/>
`environment: Minecraft`

Learning to navigate in complex environments \[2016, arxiv, Piotr Mirowski\] \[[paper](https://arxiv.org/pdf/1611.03673.pdf)\]<br/>
`method: (image --> CNN) + additional inputs (velocity, action, reward) --> stacked LSTM --> policy (A3C) + auxiliary losses (depth prediction, loop closure)`<br/>
`environment: DeepMind Lab`

Reinforcement learning with unsupervised auxiliary tasks \[2016, arxiv, Max Jaderberg\] \[[paper](https://arxiv.org/pdf/1611.05397.pdf)\]<br/>
`method: image --> CNN --> LSTM --> policy + auxiliary losses`<br/>
`environment: Labyrinth`

Deepnav: Learning to navigate large cities \[2017, CVPR, Samarth Brahmbhatt\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Brahmbhatt_DeepNav_Learning_to_CVPR_2017_paper.pdf)\]<br/>
`method: supervised learning`<br/>
`environment: Google Street View`

A deep Q network for robotic planning from image \[2017, ICARM, Jianhui Han\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8273235)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: Gazebo`

Application of deep reinforcement learning in mobile robot path planning \[2017, CAC, Jing Xin\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8244061)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: DeepMind Lab`

#### <a name="unseen">generalization</a>

Control of memory, active perception, and action in minecraft \[2016, arxiv, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1605.09128.pdf)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (DQN)`<br/>
`environment: Minecraft`

Target-driven visual navigation in indoor scenes using deep reinforcement learning \[2017, ICRA, Yuke Zhu\] \[[paper](https://arxiv.org/pdf/1609.05143.pdf,)\]<br/>
`method: (image + target image) --> ResNet50 --> generic siamese layers --> scene-specific layers: policy (A3C)`<br/>
`environment: AI2-THOR`

Transfer deep reinforcement learning in 3d environments: An empirical study \[2016, NIPS, Devendra Singh Chaplot\] \[[paper](http://www.cs.cmu.edu/~rsalakhu/papers/DeepRL_Transfer.pdf)\]<br/>
`method: image --> CNN --> policy: DQN`<br/>
`environment: VizDoom`

Neural map: Structured memory for deep reinforcement learning \[2017, arxiv, Emilio Parisotto\] \[[paper](https://arxiv.org/pdf/1702.08360.pdf)\]<br/>
`method: image --> CNN --> LSIM --> Memory --> policy (A3C)`<br/>
`environment: 2D maze, VizDoom`

Learning to navigate in cities without a map \[2018, NIPS, Piotr Mirowski\] \[[paper](https://papers.nips.cc/paper/7509-learning-to-navigate-in-cities-without-a-map.pdf)\]<br/>
`method: (image --> CNN) + (goal description, reward, action) --> LSTM --> policy (A3C) + auxiliary losses`<br/>
`environment: Google Street View`

Zero-shot visual imitation \[2018, CVPR, Deepak Pathak\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Pathak_Zero-Shot_Visual_Imitation_CVPR_2018_paper.pdf)\]<br/>
`method: ((image + goal image) --> CNN) + action --> LSTM --> policy (imitation learing) + auxiliary losses`<br/>
`environment: VizDoom`

Unsupervised predictive memory in a goal-directed agent \[2018, arxiv, Greg Wayne\] \[[paper](https://arxiv.org/pdf/1803.10760.pdf)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (A3C)`<br/>
`environment: DeepMind Lab`













