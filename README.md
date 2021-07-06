## [CCL2021幽默计算评测](https://github.com/HumorComputing/CCL2021-Humor-Computation)

### 多模态（文本+图片）
基于[kashgari](https://github.com/BrikerMan/Kashgari) / tensorflow实现  
F1过3成3就是胜利捏🤗

### 更新日志
> 2021.07.04  
>- 2天赶出第一版  
>- 图像部分直接转成3通道编码，过两层CNN  
>- 文本部分用中文BERT_base编码，过一层BiLSTM  
>- 对两个部分全局池化后的结果进行连接，过全连接层出结果  
>+ 补充：  
>> 关于task1的幽默比较，直接通过task2预测出的幽默级别进行比较，
>> 等级相同的情况下比较模型预测结果的概率值。如果概率值也相等的话（这种情况应该极少）直接认为结果为1  
>- 