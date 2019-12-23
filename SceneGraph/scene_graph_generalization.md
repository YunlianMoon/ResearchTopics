# Scene Graph Generalization

### Papers

Scene graph generation by iterative message passing \[2017, CVPR, Danfei Xu\] \[[project](https://cs.stanford.edu/~danfei/scene-graph/)\] \[[code](https://github.com/danfeiX/scene-graph-TF-release)\]<br/>
`method:` image --> faster r-cnn --> bounding boxes --> VGG16 --> (node feature --> GRU + edge feature --> GRU) --> message pooling --> object class + relationship<br/>
`dataset:` Visual Genome, NYU Depth v2

