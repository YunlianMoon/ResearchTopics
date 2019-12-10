# observation only

### Table of Contents
- Task
- Paper
  - <a href="#same">same envirionment/task</a>
  - <a href="#unseen">generalization</a>
  
### Task
Visual navigation only based on first person of view image. It integrates perception and interaction, where an agent actively interfaces with the environment to learn policies that map pixels to actions.

### Paper

#### <a name="same">same environment/task</a>

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\] \[[code](https://github.com/Ardavans/DSR)\]<br/>
`method:` image --> CNN --> --> FC --> ((FC --> w --> reward expect) + (deCNN --> observation reconstruction) + (FC --> successor representation))<br/>
`architecture:` C8x8x32 C4x4x64 C3x3x64 FC512<br/>
`environment:` MazeBase gridworld, VizDoom

A deep hierarchical approach to lifelong learning in minecraft \[2017, AAAI, Chen Tessler\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14630/13950)\]<br/>
`method:` (image --> ((CNN --> Q) + (deep skill network --> Q))) --> policy (DQN/DDQN)<br/>
`environment:` Minecraft

Learning to navigate in complex environments \[2017, ICLR, Piotr Mirowski\] \[[paper](https://arxiv.org/pdf/1611.03673.pdf)\] \[[code](https://github.com/tgangwani/GA3C-DeepNavigation)\]<br/>
`method:` (image (84*84*3) --> CNN) + additional inputs (velocity, action, reward) --> stacked LSTM --> (policy (A3C) + auxiliary losses (depth prediction, loop closure detection)) <br/>
`environment:` DeepMind Lab

Reinforcement learning with unsupervised auxiliary tasks \[2017, ICLR, Max Jaderberg\] \[[paper](https://arxiv.org/pdf/1611.05397.pdf)\] \[[code](https://github.com/miyosuda/unreal)\]<br/>
`method:` (image --> CNN + action + reward) --> FC --> LSTM --> policy (A3C) + auxiliary losses (Pixel Control, Reward Prediction, Value Function Replay)<br/>
`environment:` Labyrinth

One-shot reinforcement learning for robot navigation with interactive replay \[2017, arxiv, Jake Bruce\] \[[paper](https://arxiv.org/pdf/1711.10137.pdf)\]<br/>
`method:` images --> ResNet-50 --> FC --> FC --> LSTM --> FC --> policy (bootstrapped Q-learning/A2C/n-step Q-learning)<br/>
`environment:` office

Training agent for first-person shooter game with actor-critic curriculum learning \[2017, ICLR, Yuxin Wu\] \[[paper](https://openreview.net/pdf?id=Hk3mPK5gg)\]<br/>
`method:` images --> CNN --> FC --> (policy (A3C) + reward shaping + curriculum learning (simple to hard))<br/>
`architecture:` C7x7x32s2 C7x7x64s2 MP3x3s2 C3x3x128 MP3x3s2 C3x3x192 FC1024<br/>
`environment:` VizDoom

A deep Q network for robotic planning from image \[2017, ICARM, Jianhui Han\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8273235)\]<br/>
`method:` image --> CNN --> DQN<br/>
`environment:` Gazebo

Application of deep reinforcement learning in mobile robot path planning \[2017, CAC, Jing Xin\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8244061)\]<br/>
`method:` image --> CNN --> DQN<br/>
`environment:` DeepMind Lab

Clyde: A deep reinforcement learning DOOM playing agent \[2017, AAAI, Dino Stephen Ratcliffe\] \[[paper](https://www.aaai.org/ocs/index.php/WS/AAAIW17/paper/viewPaper/15130)\]<br/>
`method:` image --> CNN --> FC --> LSTM --> policy (A3C)<br/>
`architecture:` C8x8x16s4 MP2x2 C4x4x32s2 MP2X2 C3X3X64s1 flatten FC 512LSTM<br/>
`environment:` VizDoom

#### <a name="unseen">generalization</a>

Control of memory, active perception, and action in minecraft \[2016, ICML, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1605.09128.pdf)\] \[[code](https://github.com/junhyukoh/icml2016-minecraft)\] \[[video](https://sites.google.com/a/umich.edu/junhyuk-oh/icml2016-minecraft)\]<br/>
`method:` image --> CNN --> LSTM --> Memory --> policy (DQN)<br/>
`architecture:` C4X4X32s2p1 C4X4X64s2p1<br/>
`environment:` Minecraft

Learning to act by predicting the future \[2017, ICLR, Alexey Dosovitskiy\] \[[paper](https://arxiv.org/pdf/1611.01779.pdf)\] \[[code](https://github.com/intel-isl/DirectFuturePrediction)\] <br/>
`method:` (images --> CNN + measurements --> FC + goal --> FC) --> (expectation --> FC + action --> FC) --> policy (DFP/DQN/A3C/DSR)<br/>
`environment:` ViZDoom<br/>
code: \[[DQN](https://github.com/kuz/DeepMind-Atari-Deep-Q-Learner)\] \[[DSR](https://github.com/Ardavans/DSR)\] \[[A3C](https://github.com/muupan/async-rl)\]

Transfer deep reinforcement learning in 3d environments: An empirical study \[2016, NIPS, Devendra Singh Chaplot\] \[[paper](http://www.cs.cmu.edu/~rsalakhu/papers/DeepRL_Transfer.pdf)\]<br/>
`method:` image --> CNN --> policy (DQN)<br/>
`environment:` VizDoom

Neural map: Structured memory for deep reinforcement learning \[2018, ICLR, Emilio Parisotto\] \[[paper](https://arxiv.org/pdf/1702.08360.pdf)\]<br/>
`method:` image --> CNN --> LSIM --> Memory --> policy (A3C)<br/>
`environment:` 2D maze, VizDoom

Deep reinforcement learning with successor features for navigation across similar environments \[2017, IROS, Jingwei Zhang\] \[[paper](https://arxiv.org/pdf/1612.05533.pdf)\] \[[video](https://youtu.be/WcCcdkhgjdY)\]<br/>
`method:` images --> CNN --> FC --> ((FC --> W --> R) + (deCNN --> input construction) + (FC --> successor features) + (FC --> task map))<br/>
`environment`: maze/real

Learning to navigate in cities without a map \[2018, NIPS, Piotr Mirowski\] \[[paper](https://papers.nips.cc/paper/7509-learning-to-navigate-in-cities-without-a-map.pdf)\] \[[code](https://github.com/deepmind/streetlearn)\]<br/>
`method:` ((image --> CNN) + (goal description, reward, action)) --> LSTM --> (policy (A3C) + auxiliary losses)<br/>
`environment:` Google Street View

Zero-shot visual imitation \[2018, CVPR, Deepak Pathak\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Pathak_Zero-Shot_Visual_Imitation_CVPR_2018_paper.pdf)\] \[[code](https://github.com/pathak22/zeroshot-imitation)\]<br/>
`method:` (((image + goal image) --> CNN) + action) --> LSTM --> (policy (imitation learing) + auxiliary losses)<br/>
`environment:` VizDoom

Unsupervised predictive memory in a goal-directed agent \[2018, arxiv, Greg Wayne\] \[[paper](https://arxiv.org/pdf/1803.10760.pdf)\] \[[code](https://github.com/yosider/merlin)\]<br/>
`method:` image --> CNN --> LSTM --> Memory --> policy (A3C)<br/>
`environment:` DeepMind Lab

