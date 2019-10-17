# visual navigation using DRL

Visual semantic planning using deep successor representations \[2017, ICCV, Yuke Zhu\] \[[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Visual_Semantic_Planning_ICCV_2017_paper.pdf)\]<br/>
`method: (state(one-hot) + (image --> CNN) + (action(one-hot) --> FC) + (action augment(one-hot) --> FC)) --> FC --> (state-action feature + successor feature + reward predictor) --> (reward + Q value)`<br/>
`environment: AI2-THOR`

Visual semantic navigation using scene priors \[2018, arxiv, Wei Yang\] \[[paper](https://arxiv.org/pdf/1810.06543.pdf)\] \[[video](incorporating)\]<br/>
`method: ((images --> ResNet50 --> FC) + (goal --> word embedding --> FC) + (graph knowledge --> GCN --> FC)) --> FC --> policy (A3C)`<br/>
`environment: AI2-THOR`

Understanding grounded language learning agents \[2017, arxiv, Felix Hill\] \[[paper](https://arxiv.org/pdf/1710.09867.pdf)\]<br/>
`method: ((image --> CNN) + (textual instruction) --> LSTM) --> FC --> LSTM --> policy (A3C)`<br/>
`environment: DeepMind Lab`

Zero-shot task generalization with multi-task deep reinforcement learning \[2017, ICML, Junhyuk Oh\] \[[paper](https://arxiv.org/pdf/1706.05064.pdf)\] \[[video](https://sites.google.com/a/umich.edu/junhyuk-oh/task-generalization)\]<br/>
`method: (((instructions + image) --> meta controller (CNN + LSTM)) + image) --> paremetrirized sill (CNN + LSTM) --> policy (A2C) + termination prediction`<br/>
`environment: Minecraft`

Grounded language learning in a simulated 3d world \[2017, arxiv, Karl Moritz Hermann\] \[[paper](https://arxiv.org/pdf/1706.06551.pdf)\] \[[code](https://github.com/dai-dao/Grounded-Language-Learning-in-Pytorch)\]<br/>
`method: ((image --> CNN) + (textual instruction --> LSTM)) --> NN --> LSTM --> (policy (A3C) + autoencoder auxiliary task + language      prediction)`<br/>
`environment: DeepMind Lab`

Gated-attention architectures for task-oriented language grounding \[2018, AAAI, Devendra Singh Chaplot\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/viewFile/17425/16578)\] \[[code](https://github.com/devendrachaplot/DeepRL-Grounding)\]<br/>
`description: unseen instructions/maps`<br/>
`method: ((image --> CNN) + (text instruction --> GRU --> FC --> attention vector)) --> FC --> LSTM --> (policy (A3C) + imitation learning (behavioral cloning/DAgger))`<br/>
`environment: ViZDoom`
