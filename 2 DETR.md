# End-to-End Object Detection with Transformers
![title](images/2-1.PNG)<br>
作者单位：Facebook AI<br>
文章链接：[paper](https://arxiv.org/pdf/2005.12872v3.pdf), [code](https://github.com/facebookresearch/detr)<br>
会议：ECCV2020<br>

## 摘要
本文解决目标检测的方法是集合预测，网络的输出就是最终的预测的集合，也不需要任何后处理。
集合预测简化了检测的流程，不需要NMS以及预设anchor。
新框架名为DETR（检测transformer），其中的主要构成有：基于集合的全局损失；transformer的编码器-解码器结构。
当指定一组可学习的目标“查询-query”，DETR推理出目标和全局信息的关系，直接输出所有预测结果。
在COCO数据集上，DETR的精度和运行速度都与Faster R-CNN不相上下，并且可以扩展到全景分割的任务。
