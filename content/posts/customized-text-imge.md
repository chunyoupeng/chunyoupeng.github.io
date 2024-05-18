
# Problem

Users wish to synthesize specific concepts from their own personal lives.用户想要定制自己的主题。但是现有的模型很难产生未看到的背景。

# Assumption in prior work

Prior work improves compositional generation to extend beyond tuning for a single, individual concept and compose multiple conceots together, but they lead addtional chanllenges as mixing unseen concepts.

# Insight

他们识别出了小部份的模型权重，通过稍调这些小部分的权重就足够更新模型适应新的图像概念。
augmentation
他们提出的方法可以分别训练然后合并。


# Technical overview

该方法支持训练多个概念并在新颖的环境中将它们组合起来，同时生成现有概念的新变体。该方法优于几个基准和同时进行的工作，在定性和定量评估中表现出色，同时具有计算和内存效率。

# Proof



## 结果比较

![single-concept](/img/single-concept.png ) 
> 单概念微调结果比较

他们的模型可以生成背景和艺术风格。以第一行为例，生成一个水彩风格的在山上的乌龟。他们的模型能产生山的背景，而其它的比如DreamBooth和Textual Inversion则不行，效果较差。

![multi-concept](/img/multi-concept.png ) 
>多概念微调结果比较

在多概念的情况下，也就是把多个主题融合起来。从上图可以看到，他们的模型有更高的视觉相似度（两个或多个视觉对象在视觉特征上的相似度）。然而DreamBooth有时会忽略掉猫。

### 量化比较


![quantitative-cmp](/img/quantitative-cmp.png )
>上面的结果表明，不管是单概念还是多概念都要优于DreamBooth

 本文提出了一种在新概念、类别、个人对象或艺术风格上微调大规模文本到图像扩散模型的方法，只使用少量图像示例。该方法在新环境中生成微调概念的新变体，保持与目标图像的视觉相似性。它还可以在同一场景中组合多个新概念，并在背景中生成山脉。该方法在每个组合设置的8个提示生成的400个图像上优于其他基准。人类偏好研究表明，所提出的方法在单一概念和多概念方面优于基准。该方法在难以组合的情况下显示出局限性，例如宠物狗和猫，以及组合三个或更多概念。

# Impact

他们提出了种新方法用来微调大规模文生图的扩散模型，只需要几个图片就可以生成新的概念，主题和艺术风格。他们的优点如下：
1. 高效计算
2. 只需要小部份的权重就可以进行训练
