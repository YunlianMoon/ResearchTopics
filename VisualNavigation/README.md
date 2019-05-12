# Visual Navigation using DRL

### Table of Contents
- Survey
- Paper
  - <a href="#image">image</a>
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

Deep successor reinforcement learning \[2016, arxiv, Tejas D. Kulkarni\] \[[paper](https://arxiv.org/pdf/1606.02396.pdf)\]
`method: image --> CNN --> successor representation (SR)`
`Environment: MazeBase gridworld, VizDoom`

Control of memory, active perception, and action in minecraft \[2016, arxiv, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1605.09128.pdf)\]

Towards cognitive exploration through deep reinforcement learning for mobile robots \[2016, arxiv, Lei Tai\] \[[paper](https://arxiv.org/pdf/1610.01733.pdf)\]

Deep reinforcement learning in a 3-d blockworld environment \[2016, IJCAI, Trevor Barron\] \[[paper](http://cs.coloradocollege.edu/~mwhitehead/files/mypapers/blockworld.pdf)\]

Learning to navigate in complex environments \[2016, arxiv, Piotr Mirowski\] \[[paper](https://arxiv.org/pdf/1611.03673.pdf)\]

`method: (image --> CNN) + additional inputs (velocity, action, reward) --> policy + auxiliary losses (depth prediction, loop closure)`

Target-driven visual navigation in indoor scenes using deep reinforcement learning \[2017, ICRA, Yuke Zhu\] \[[paper](https://arxiv.org/pdf/1609.05143.pdf,)\]




