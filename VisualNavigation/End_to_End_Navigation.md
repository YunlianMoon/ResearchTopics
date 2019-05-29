# End to End Visual Navigation

## Table of Contents
- <a href="#VLN">vision and language</a>
  - <a href="#instruction">instruction</a>


## <a name="VLN">vision and language</a>

### <a name="instruction">instruction</a>

Speaker-follower models for vision-and-language navigation \[2018, NIPS, Daniel Fried\] \[[paper](https://papers.nips.cc/paper/7592-speaker-follower-models-for-vision-and-language-navigation.pdf)\]<br/>
`description: unseen environment`<br/>
`method: fllower module + speaker module`<br/>
`method: ((route description --> LSTM --> attention) + (images --> ResNet --> LSTM --> attention)) --> action)`
`environment: R2R`
