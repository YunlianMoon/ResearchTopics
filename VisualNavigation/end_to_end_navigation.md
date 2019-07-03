# End to End Visual Navigation

### Table of Contents
- <a href="#VLN">vision and language</a>
  - <a href="#semantic">semantic</a>
  - <a href="#instruction">instruction</a>

### <a name="VLN">vision and language</a>

#### <a name="semantic">semantic</a>
Visual representations for semantic target driven navigation \[2018, ECCV, Arsalan Mousavian\] \[[paper](https://arxiv.org/pdf/1805.06066.pdf)\] \[[code](https://github.com/tensorflow/models/tree/master/research/cognitive_planning)\]<br/>
`topic: object goal`
`description: reward (distance)`<br/>
`method: (((((object detection + semantic segmentation + depth image) --> CNN) + (image --> ResNet50)) --> FC) + goal (one-hot) + action + success binary indicator (colison)) --> LSTM --> FC --> cost v`<br/>
`environment: SUNCG, AVD`

#### <a name="instruction">instruction</a>

Listen, attend, and walk: Neural mapping of navigational instructions to action sequences \[2016, AAAI, Hongyuan Mei\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/viewFile/12522/12021)\]<br/>
`topic: instruction`

Speaker-follower models for vision-and-language navigation \[2018, NIPS, Daniel Fried\] \[[paper](https://papers.nips.cc/paper/7592-speaker-follower-models-for-vision-and-language-navigation.pdf)\]<br/>
`description: unseen environment`<br/>
`method: fllower module + speaker module`<br/>
`method: ((route description --> LSTM --> attention) + (images --> ResNet --> LSTM --> attention)) --> action)`
`environment: R2R`
