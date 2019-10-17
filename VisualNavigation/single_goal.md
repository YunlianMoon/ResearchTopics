# Visual Navigation using DRL

most single goal visual navigation trained in game environments.

### Paper

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\] \[[code](https://github.com/Ardavans/DSR)\]<br/>
`method: image --> CNN --> --> FC --> ((FC --> w --> reward expect) + (deCNN --> observation reconstruction) + (FC --> successor representation))`<br/>
`architecture: C8x8x32 C4x4x64 C3x3x64 FC512`<br/>
`environment: MazeBase gridworld, VizDoom`

A deep hierarchical approach to lifelong learning in minecraft \[2017, AAAI, Chen Tessler\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14630/13950)\]<br/>
`method: (image --> ((CNN --> Q) + (deep skill network --> Q))) --> policy (DQN/DDQN)`<br/>
`environment: Minecraft`

Learning to navigate in complex environments \[2017, ICLR, Piotr Mirowski\] \[[paper](https://arxiv.org/pdf/1611.03673.pdf)\] \[[code](https://github.com/tgangwani/GA3C-DeepNavigation)\]<br/>
`method: (image (84*84*3) --> CNN) + additional inputs (velocity, action, reward) --> stacked LSTM --> (policy (A3C) + auxiliary losses (depth prediction, loop closure detection))` <br/>
`environment: DeepMind Lab`

Reinforcement learning with unsupervised auxiliary tasks \[2017, ICLR, Max Jaderberg\] \[[paper](https://arxiv.org/pdf/1611.05397.pdf)\] \[[code](https://github.com/miyosuda/unreal)\]<br/>
`method: (image --> CNN + action + reward) --> FC --> LSTM --> policy (A3C) + auxiliary losses (Pixel Control, Reward Prediction, Value Function Replay)`<br/>
`environment: Labyrinth`

One-shot reinforcement learning for robot navigation with interactive replay \[2017, arxiv, Jake Bruce\] \[[paper](https://arxiv.org/pdf/1711.10137.pdf)\]<br/>
`method: images --> ResNet-50 --> FC --> FC --> LSTM --> FC --> policy (bootstrapped Q-learning/A2C/n-step Q-learning)`<br/>
`environment: office`

Training agent for first-person shooter game with actor-critic curriculum learning \[2017, ICLR, Yuxin Wu\] \[[paper](https://openreview.net/pdf?id=Hk3mPK5gg)\]<br/>
`method: images --> CNN --> FC --> (policy (A3C) + reward shaping + curriculum learning (simple to hard))`<br/>
`architecture: C7x7x32s2 C7x7x64s2 MP3x3s2 C3x3x128 MP3x3s2 C3x3x192 FC1024`<br/>
`environment: VizDoom`

A deep Q network for robotic planning from image \[2017, ICARM, Jianhui Han\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8273235)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: Gazebo`

Application of deep reinforcement learning in mobile robot path planning \[2017, CAC, Jing Xin\] \[[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8244061)\]<br/>
`method: image --> CNN --> DQN`<br/>
`environment: DeepMind Lab`

Clyde: A deep reinforcement learning DOOM playing agent \[2017, AAAI, Dino Stephen Ratcliffe\] \[[paper](https://www.aaai.org/ocs/index.php/WS/AAAIW17/paper/viewPaper/15130)\]<br/>
`method: image --> CNN --> FC --> LSTM --> policy (A3C)`<br/>
`architecture: C8x8x16s4 MP2x2 C4x4x32s2 MP2X2 C3X3X64s1 flatten FC 512LSTM`<br/>
`environment: VizDoom`
