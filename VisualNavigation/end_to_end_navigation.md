# End to End Visual Navigation

### Table of Contents
- <a href="#VLN">vision and language</a>
  - <a href="#instruction">instruction</a>


### <a name="VLN">vision and language</a>

#### <a name="instruction">instruction</a>

Listen, attend, and walk: Neural mapping of navigational instructions to action sequences \[2016, AAAI, Hongyuan Mei\] \[[paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/viewFile/12522/12021)\]<br/>
`topic: instruction`

Speaker-follower models for vision-and-language navigation \[2018, NIPS, Daniel Fried\] \[[paper](https://papers.nips.cc/paper/7592-speaker-follower-models-for-vision-and-language-navigation.pdf)\]<br/>
`description: unseen environment`<br/>
`method: fllower module + speaker module`<br/>
`method: ((route description --> LSTM --> attention) + (images --> ResNet --> LSTM --> attention)) --> action)`
`environment: R2R`
