# instruction

### paper

Mapping instructions and visual observations to actions with reinforcement learning \[2017, arxiv, Dipendra Misra\] \[[paper](https://arxiv.org/pdf/1704.08795.pdf)\] \[[code](https://github.com/lil-lab/blocks)\]<br/>
`method: ((image --> CNN) + (instruction --> LSTM) + (action --> NN)) --> NN --> policy (policy gradient)`<br/>
`environment: block world`

Vision-and-language navigation: Interpreting visually-grounded navigation instructions in real environments \[2018, CVPR, Peter Anderson\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Anderson_Vision-and-Language_Navigation_Interpreting_CVPR_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: ((instruction --> LSTM) + ((image --> ResNet152 + action) --> LSTM)) --> attention --> teacher-forcing/student-forcing`<br/>
`environment: R2R`

Scheduled policy optimization for natural language communication with intelligent agents \[2018, arxiv, Wenhan Xiong\] \[[Paper](https://arxiv.org/pdf/1806.06187.pdf)\]<br/>
`mehtod: (image --> CNN + instruction --> LSTM + action --> NN) --> policy (imitation learning + PPO/REINFORCE/A2C/DQN)`<br/>
`environment: block-world`

Look before you leap: Bridging model-free and model-based reinforcement learning for planned-ahead vision-and-language navigation \[2018, ECCV, Xin Wang\] \[[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xin_Wang_Look_Before_You_ECCV_2018_paper.pdf)\]<br/>
`description: unseen environments`<br/>
`method: model-free + model-based`<br/>
`method: ((image --> CNN) + (instruction --> attention --> LSTM) ) --> LSTM --> policy (REINFORCE)`<br/>
`environment: R2R`

Reinforced Cross-Modal Matching and Self-Supervised Imitation Learning for Vision-Language Navigation \[2018, arxiv, Xin Wang\] \[[paper](https://arxiv.org/pdf/1811.10092.pdf)\]<br/>
`description: unseen environments`<br/>
`reward: Extrinsic Reward (relative navigation distance/success) + Intrinsic Reward (instruction reconstruction)`<br/>
`method: (textual instruction --> LSTM + (images --> ResNet152 --> attention + action) --> LSTM) --> attention --> policy (imitation learning + REINFORCE)`<br/>
`environment: R2R`
