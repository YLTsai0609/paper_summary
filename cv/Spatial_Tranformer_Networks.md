# Spatial_Tranformer_Networks

[paper](https://proceedings.neurips.cc/paper/2015/file/33ceb07bf4eeb3da587e268d663aba1a-Paper.pdf)

[github](https://github.com/kevinzakka/spatial-transformer-network)

Max Jaderberg

Karen Simonyan

Andrew Zisserman

koray kavukcuoglu

# 摘要

CNN是一個表現力相當好的模型，但是這個模型仍然缺乏空間不變性(spatially invariant)，不論在參數上或是算力上都是[註1]，這篇Paper我們要介紹一個新的網路架構 Spatial Transfer，這個網路架構允許資料在網路裡面進行空間變換，而且是可微分的，可以被接在任何的Convolutional architechture裡面，讓神經網路擁有對feature maps進行空間變換的能力，不需要多增加新的data或是修正最佳化過程，作者們使用了spatial transformer來學習圖片的仿射變換，包含平移，伸縮，巡轉以及更多廣義仿射，達到了當前的最好表現(state-of-the-art performance on several nenchmarks)

# 被激發的像法

註1 : 顯然這既是為什麼目前我們使用Data Augmentation時 zoom in zoom out 旋轉 仍然提昇了不少performance的原因

## From 李弘毅課程

[Advanced Topics in Deep Learning, Spatial Tranformer Layer](https://www.youtube.com/watch?v=SoCywZ1hZak)
