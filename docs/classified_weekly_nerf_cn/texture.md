
每周分类神经辐射场 - texture ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
====================================================================================================================================
## 按类别筛选: 
 [全部](../weekly_nerf_cn.md) | [动态](./dynamic.md) | [编辑](./editing.md) | [快速](./fast.md) | [泛化](./generalization.md) | [人体](./human.md) | [视频](./video.md) | [光照](./lighting.md) | [重建](./reconstruction.md) | [纹理](./texture.md) | [语义](./semantic.md) | [姿态-SLAM](./pose-slam.md) | [其他](./others.md) 
## Aug21 - Aug27, 2022
## Aug14 - Aug20, 2022
## Aug7 - Aug13, 2022
## Jul31 - Aug6, 2022
## Jul24 - Jul30, 2022
  - [ShAPO：多对象形状、外观和姿势优化的隐式表示, ECCV2022](https://arxiv.org/abs/2207.13691) | [***``[code]``***](https://zubair-irshad.github.io/projects/ShAPO.html)
    > 我们的方法从单个 RGB-D 观察中研究以对象为中心的 3D 理解的复杂任务。由于这是一个不适定问题，现有方法在具有遮挡的复杂多对象场景中的 3D 形状和 6D 姿势和尺寸估计性能低下。我们提出了 ShaAPO，一种用于联合多对象检测、3D 纹理重建、6D 对象姿态和大小估计的方法。 ShAPO 的关键是一个单次管道，用于回归形状、外观和姿势潜在代码以及每个对象实例的掩码，然后以稀疏到密集的方式进一步细化。首先学习了一种新的解开的先验形状和外观数据库，以将对象嵌入到它们各自的形状和外观空间中。我们还提出了一种新颖的、基于八叉树的可微优化步骤，使我们能够以综合分析的方式在学习的潜在空间下同时进一步改进对象形状、姿势和外观。我们新颖的联合隐式纹理对象表示使我们能够准确地识别和重建新的看不见的对象，而无需访问它们的 3D 网格。通过广泛的实验，我们证明了我们的方法在模拟室内场景上进行训练，能够以最少的微调准确地回归现实世界中新物体的形状、外观和姿势。我们的方法显着优于 NOCS 数据集上的所有基线，6D 姿态估计的 mAP 绝对提高了 8%。
  - [NeuMesh：学习基于解缠结神经网格的隐式场，用于几何和纹理编辑, ECCV2022(oral)](https://arxiv.org/abs/2207.11911) | [code]
    > 最近，神经隐式渲染技术得到了迅速发展，并在新颖的视图合成和 3D 场景重建中显示出巨大的优势。然而，现有的用于编辑目的的神经渲染方法提供的功能有限，例如，刚性变换，或者不适用于日常生活中一般对象的细粒度编辑。在本文中，我们提出了一种新颖的基于网格的表示，通过在网格顶点上使用解开几何和纹理代码对神经隐场进行编码，这促进了一组编辑功能，包括网格引导的几何编辑、带有纹理交换的指定纹理编辑、填充和绘画操作。为此，我们开发了几种技术包括可学习的符号指标以放大基于网格的表示的空间可区分性，蒸馏和微调机制以实现稳定收敛，以及空间感知优化策略以实现精确的纹理编辑。对真实数据和合成数据的大量实验和编辑示例证明了我们的方法在表示质量和编辑能力方面的优越性。代码可在项目网页上找到：此 https URL。
## Previous weeks
  - [CodeNeRF：对象类别的解开神经辐射场, ICCV2021(oral)](https://www.google.com/url?q=https%3A%2F%2Farxiv.org%2Fpdf%2F2109.01750.pdf&sa=D&sntz=1&usg=AOvVaw1Fnir0e4aRa22Nt0HoXDWh) | [***``[code]``***](https://www.google.com/url?q=https%3A%2F%2Fgithub.com%2Fwbjang%2Fcode-nerf&sa=D&sntz=1&usg=AOvVaw2eD5ZoRbk2aWFuwUSHlh5_)
    > CodeNeRF 是一种隐式 3D 神经表示，它学习对象形状和纹理在一个类别中的变化，并且可以从一组姿势图像中进行训练，以合成看不见的对象的新视图。与特定场景的原始 NeRF 不同，CodeNeRF 通过学习单独的嵌入来学习解开形状和纹理。在测试时，给定一个看不见的物体的单个未定位图像，CodeNeRF 通过优化联合估计相机视点、形状和外观代码。看不见的物体可以从单个图像中重建，然后从新的视点渲染，或者通过改变潜在代码编辑它们的形状和纹理。我们在 SRN 基准上进行了实验，结果表明 CodeNeRF 可以很好地泛化到看不见的对象，并且在测试时需要已知相机姿态的方法达到同等性能。我们在真实世界图像上的结果表明，CodeNeRF 可以弥合模拟到真实的差距。
  - [物体辐射场的无监督发现, ICLR2022](https://arxiv.org/abs/2107.07905) | [code]
    > 我们研究从单个图像推断以对象为中心的场景表示的问题，旨在推导出解释图像形成过程的表示，捕捉场景的 3D 性质，并且在没有监督的情况下学习。由于将复杂的 3D 到 2D 图像形成过程集成到强大的推理方案（如深度网络）中存在根本性挑战，大多数现有的场景分解方法都缺乏这些特征中的一个或多个。在本文中，我们提出了对象辐射场 (uORF) 的无监督发现，将神经 3D 场景表示和渲染的最新进展与深度推理网络相结合，用于无监督 3D 场景分解。在没有注释的多视图 RGB 图像上进行训练，uORF 学习从单个图像分解具有不同纹理背景的复杂场景。我们展示了 uORF 在无监督 3D 场景分割、新视图合成和三个数据集上的场景编辑方面表现良好。
  - [NeRF-Tex：神经反射场纹理, EGSR2021](https://developer.nvidia.com/blog/nvidia-research-nerf-tex-neural-reflectance-field-textures/) | [***``[code]``***](https://github.com/hbaatz/nerf-tex)
    > 我们研究使用神经场来模拟不同的中尺度结构，例如毛皮、织物和草。我们建议使用由神经反射场 (NeRF-Tex) 表示的多功能体积基元，而不是使用经典的图形基元来建模结构，它联合建模材料的几何形状及其对照明的响应。 NeRF-Tex 原语可以在基础网格上实例化，以使用所需的细观和微尺度外观对其进行“纹理化”。我们根据控制外观的用户定义参数来调节反射率场。因此，单个 NeRF 纹理捕获了反射场的整个空间，而不是一个特定的结构。这增加了可以建模的外观范围，并提供了一种解决重复纹理伪影的解决方案。我们还证明了 NeRF 纹理自然地促进了连续的细节层次渲染。我们的方法将神经网络的多功能性和建模能力与虚拟场景精确建模所需的艺术控制相结合。虽然我们所有的训练数据目前都是合成的，但我们的工作提供了一个方法，可以进一步扩展以从真实图像中提取复杂、难以建模的外观。
