# Scene Graph Generation

### Papers

Knowledge-Embedded Routing Network for Scene Graph Generation \[2019, CVPR, Tianshui Chen\] \[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Chen_Knowledge-Embedded_Routing_Network_for_Scene_Graph_Generation_CVPR_2019_paper.pdf)\]

Learning to compose dynamic tree structures for visual contexts \[2019, CVPR, Kaihua Tang\] \[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Tang_Learning_to_Compose_Dynamic_Tree_Structures_for_Visual_Contexts_CVPR_2019_paper.pdf)\] \[[code](https://github.com/KaihuaTang/VCTree-Scene-Graph-Generation)\]

Neural motifs: Scene graph parsing with global context \[2018, CVPR, Rowan Zellers\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zellers_Neural_Motifs_Scene_CVPR_2018_paper.pdf)\] \[[code](https://github.com/rowanz/neural-motifs)\]<br/>
`method:` image --> fast r-cnn --> bounding boxes --> VGG --> bidirectional LSTMs --> LSTM --> bidirectional LSTMs --> relation<br/>
`dataset:` Visual Genome

Graph r-cnn for scene graph generation \[2018, ECCV, Jianwei Yang\] \[[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Jianwei_Yang_Graph_R-CNN_for_ECCV_2018_paper.pdf)\] \[[code](https://github.com/jwyang/graph-rcnn.pytorch)\]

Factorizable net: an efficient subgraph-based framework for scene graph generation \[2018, ECCV, Yikang LI\] \[[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Yikang_LI_Factorizable_Net_An_ECCV_2018_paper.pdf)\] \[[code](https://github.com/yikang-li/FactorizableNet)\]

Mapping images to scene graphs with permutation-invariant structured prediction \[2018, NIPS, Roei Herzig\] \[[paper](https://papers.nips.cc/paper/7951-mapping-images-to-scene-graphs-with-permutation-invariant-structured-prediction.pdf)\]

Linknet: Relational embedding for scene graph \[2018, NIPS, Sanghyun Woo\] \[[paper](https://papers.nips.cc/paper/7337-linknet-relational-embedding-for-scene-graph.pdf)\]

Scene graph generation by iterative message passing \[2017, CVPR, Danfei Xu\] \[[project](https://cs.stanford.edu/~danfei/scene-graph/)\] \[[code](https://github.com/danfeiX/scene-graph-TF-release)\]<br/>
`method:` image --> faster r-cnn --> bounding boxes --> VGG16 --> (node feature --> GRU + edge feature --> GRU) --> message pooling --> object class + relationship<br/>
`dataset:` Visual Genome, NYU Depth v2

Scene graph generation from objects, phrases and region captions \[2017, ICCV, Yikang Li\] \[[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Li_Scene_Graph_Generation_ICCV_2017_paper.pdf)\] \[[code](https://github.com/yikang-li/MSDN)\]

Detecting visual relationships with deep relational networks \[2017, CVPR, Bo Dai\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Dai_Detecting_Visual_Relationships_CVPR_2017_paper.pdf)\] \[[code](https://github.com/doubledaibo/drnet_cvpr2017)\]

Visual translation embedding network for visual relation detection \[2017, CVPR, Hanwang Zhang\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Zhang_Visual_Translation_Embedding_CVPR_2017_paper.pdf)\] \[[code](https://github.com/zawlin/cvpr17_vtranse)\]

Vip-cnn: Visual phrase guided convolutional neural network \[2017, CVPR, Yikang Li\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Li_ViP-CNN_Visual_Phrase_CVPR_2017_paper.pdf)\]

Deep variation-structured reinforcement learning for visual relationship and attribute detection \[2017, CVPR, Xiaodan Liang\] \[[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Liang_Deep_Variation-Structured_Reinforcement_CVPR_2017_paper.pdf)\]

Pixels to graphs by associative embedding \[2017, NIPS, Alejandro Newell\] \[[paper](http://papers.nips.cc/paper/6812-pixels-to-graphs-by-associative-embedding.pdf)\] \[[code](https://github.com/princeton-vl/px2graph)\]

Visual relationship detection with language priors \[2016, ECCV, Cewu Lu\] \[[paper](https://www-cs.stanford.edu/people/ranjaykrishna/vrd/vrd.pdf)\] \[[code](https://github.com/Prof-Lu-Cewu/Visual-Relationship-Detection)\]



