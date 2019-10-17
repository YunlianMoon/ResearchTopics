# Visual Navigation using DRL

most single goal visual navigation trained in game environments.

### Paper

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\] \[[code](https://github.com/Ardavans/DSR)\]<br/>
`method: image --> CNN --> --> FC --> ((FC --> w --> reward expect) + (deCNN --> observation reconstruction) + (FC --> successor representation))`<br/>
`architecture: C8x8x32 C4x4x64 C3x3x64 FC512`<br/>
`environment: MazeBase gridworld, VizDoom`


