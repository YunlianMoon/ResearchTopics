# visual navigation using DRL

Control of memory, active perception, and action in minecraft \[2016, ICML, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1605.09128.pdf)\] \[[code](https://github.com/junhyukoh/icml2016-minecraft)\] \[[video](https://sites.google.com/a/umich.edu/junhyuk-oh/icml2016-minecraft)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (DQN)`<br/>
`architecture: C4X4X32s2p1 C4X4X64s2p1`<br/>
`environment: Minecraft`

Learning to act by predicting the future \[2017, ICLR, Alexey Dosovitskiy\] \[[paper](https://arxiv.org/pdf/1611.01779.pdf)\] \[[code](https://github.com/intel-isl/DirectFuturePrediction)\] <br/>
`method: (images --> CNN + measurements --> FC + goal --> FC) --> (expectation --> FC + action --> FC) --> policy (DFP/DQN/A3C/DSR)`<br/>
`environment: ViZDoom` <br/>
code: \[[DQN](https://github.com/kuz/DeepMind-Atari-Deep-Q-Learner)\] \[[DSR](https://github.com/Ardavans/DSR)\] \[[A3C](https://github.com/muupan/async-rl)\]

Target-driven visual navigation in indoor scenes using deep reinforcement learning \[2017, ICRA, Yuke Zhu\] \[[paper](https://arxiv.org/pdf/1609.05143.pdf,)\] \[[code](https://github.com/yushu-liu/icra2017-visual-navigation)\]<br/>
`method: (image + target image) --> ResNet50 --> generic siamese layers --> scene-specific layers --> policy (A3C)`<br/>
`environment: AI2-THOR`

Transfer deep reinforcement learning in 3d environments: An empirical study \[2016, NIPS, Devendra Singh Chaplot\] \[[paper](http://www.cs.cmu.edu/~rsalakhu/papers/DeepRL_Transfer.pdf)\]<br/>
`method: image --> CNN --> policy (DQN)`<br/>
`environment: VizDoom`

Neural map: Structured memory for deep reinforcement learning \[2018, ICLR, Emilio Parisotto\] \[[paper](https://arxiv.org/pdf/1702.08360.pdf)\]<br/>
`method: image --> CNN --> LSIM --> Memory --> policy (A3C)`<br/>
`environment: 2D maze, VizDoom`

Deep reinforcement learning with successor features for navigation across similar environments \[2017, IROS, Jingwei Zhang\] \[[paper](https://arxiv.org/pdf/1612.05533.pdf)\] \[[video](https://youtu.be/WcCcdkhgjdY)\]<br/>
`method: images --> CNN --> FC --> ((FC --> W --> R) + (deCNN --> input construction) + (FC --> successor features) + (FC --> task map))`<br/>
`environment: maze/real

Learning to navigate in cities without a map \[2018, NIPS, Piotr Mirowski\] \[[paper](https://papers.nips.cc/paper/7509-learning-to-navigate-in-cities-without-a-map.pdf)\] \[[code](https://github.com/deepmind/streetlearn)\]<br/>
`method: ((image --> CNN) + (goal description, reward, action)) --> LSTM --> (policy (A3C) + auxiliary losses)`<br/>
`environment: Google Street View`

Zero-shot visual imitation \[2018, CVPR, Deepak Pathak\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Pathak_Zero-Shot_Visual_Imitation_CVPR_2018_paper.pdf)\] \[[code](https://github.com/pathak22/zeroshot-imitation)\]<br/>
`method: (((image + goal image) --> CNN) + action) --> LSTM --> (policy (imitation learing) + auxiliary losses)`<br/>
`environment: VizDoom`

Unsupervised predictive memory in a goal-directed agent \[2018, arxiv, Greg Wayne\] \[[paper](https://arxiv.org/pdf/1803.10760.pdf)\] \[[code](https://github.com/yosider/merlin)\]<br/>
`method: image --> CNN --> LSTM --> Memory --> policy (A3C)`<br/>
`environment: DeepMind Lab`
