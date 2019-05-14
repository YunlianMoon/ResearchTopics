# Visual Navigation using DRL

### Table of Contents
- Survey
- Paper
  - <a href="#image">image</a>
  - <a href="#VLN">vision and language</a>
    - <a href="#PG">point goal</a>
    - <a href="#OG">object goal</a>
    - <a href="#AG">area goal</a>
    - <a href="#instruction">instruction</a>
    - <a href="#question">question</a>

#### <a name="OG">object goal</a>

Visual semantic planning using deep successor representations \[2017, ICCV, Yuke Zhu\] \[[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Visual_Semantic_Planning_ICCV_2017_paper.pdf)\]<br/>
`method: image + action --> CNN --> successor representation (SR)`<br/>
`environment: AI2-THOR`

Visual representations for semantic target driven navigation \[2018, arxiv, Arsalan Mousavian\] \[[paper](https://arxiv.org/pdf/1805.06066.pdf)\]<br/>
`description: reward (distance)`<br/>
`method: ((image --> ResNet50) + target (one-hot) + action + success binary indicator (colison) + object detection + semantic segmentation + depth image) --> CNN --> LSTM --> NN --> policy (imitation learning + DQN)`<br/>
`environment: SUNCG, AVD`

Visual semantic navigation using scene priors \[2018, arxiv, Wei Yang\] \[[paper](https://arxiv.org/pdf/1810.06543.pdf)\]<br/>
`method: ((4 history images --> ResNet50) + (goal --> word embedding) + (graph knowledge --> GCN)) --> NN --> policy (A3C)`<br/>
`environment: AI2-THOR`

#### <a name="instruction">instruction</a>

Listen, attend, and walk: Neural mapping of navigational instructions to action sequences \[2016, AAAI, Hongyuan Mei\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/viewFile/12522/12021)\]

Understanding grounded language learning agents \[2017, arxiv, Felix Hill\] \[[paper](https://arxiv.org/pdf/1710.09867.pdf)\]

#### <a name="question">question</a>




