# High Efficiency Deep Joint Source-Channel Coding for One-to-Many Wireless Image Transmission

This is the code for paper "High Efficiency Deep Joint Source-Channel Coding for One-to-Many Wireless Image Transmission". The model is implemented with PyTorch.

# Abstruct

Deep learning based joint source-channel coding (DJSCC) has recently made significant progress and emerged as a potential solution for future wireless communications. However, there are still several crucial issues that necessitate further in-depth exploration to enhance the efficiency of DJSCC, such as channel quality adaptability, bandwidth adaptability, and the delicate balance between efficiency and complexity. This work proposes a high efficiency deep joint source-channel coding scheme (MDJSCC) tailored for one-to-many wireless transmission scenarios. First, to effectively improve transmission performance, neighboring attention is introduced as the backbone for the proposed MDJSCC method. Second,  a channel quality adaptive module(CQAM) is designed based on multi-scale feature fusion, which seamlessly adapts to fluctuating channel conditions across a wide range of channel signal-to-noise ratios (CSNRs). Third, to be precisely tailored to different bandwidth resources, the channel gained adaptive module (CGAM) dynamically adjusts the significance of individual channels within the latent space, which ensures seamless varying bandwidth accommodation with a single model through bandwidth adaptation and symbol completion. Additionally, to mitigate the imbalance of loss across multiple bandwidth ratios during the training process, the gradient normalization (GradNorm) based training strategy is leveraged to ensure adaptive loss balancing. The extensive experimental results demonstrate that the proposed method significantly enhances transmission performance while maintaining relatively low computational complexity.

# Pipline

<div align="center">
  <img src="Sys_model2.png" width="85%">
</div>

<div align="center">
  <img src="fig_network_overview.png" width="85%">
</div>

# Usage

## Requirements

```
git clone https://github.com/llsurreal919/MDJSCC

pip install -r requirements.txt
```

## Dataset

The test dataset can be downloaded from [kaggle](https://www.kaggle.com/datasets/drxinchengzhu/kodak24) .

The training dataset can be downloaded from [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/) .

## Training

We will release the tutorial soon.

## Testing

Pre-trained models can be downloaded from [GoogleDrive](https://drive.google.com/file/d/1o7aqd5OgAIltr8NK6tmF-jkeq7xmc1HS/view?usp=sharing).

Example usage:

    python test_dyna_kodak.py

# Acknowledgement

The style of coding is borrowed from [Dynamic_JSCC](https://github.com/mingyuyng/Dynamic_JSCC) and partially built upon the [Neighborhood Attention Transformer](https://github.com/SHI-Labs/Neighborhood-Attention-Transformer). We thank the authors for sharing their codes.

# Related work
> He Ziyang, Huang Minfeng, Luo Lei, Yang Xu and Zhu Ce, "Efficient Deep Visual and Inertial Odometry with Adaptive Visual Modality Selection"
```
  @article{he2024towards,
    title={Towards real-time practical image compression with lightweight attention},
    author={He, Ziyang and Huang, Minfeng and Luo, Lei and Yang, Xu and Zhu, Ce},
    journal={Expert Systems with Applications},
    volume={252},
    pages={124142},
    year={2024},
    publisher={Elsevier}
  }
```
> Cheng Baoping, Luo Lei, He Ziyang, Zhu Ce and Tao Xiaoming, "Perceptual point cloud qality assessment for immersive metaverse experience"
```
  @article{cheng2024perceptual,
    title={Perceptual point cloud qality assessment for immersive metaverse experience},
    author={Cheng, Baoping and Luo, Lei and He, Ziyang and Zhu, Ce and Tao, Xiaoming},
    journal={Digital Communications and Networks},
    year={2024},
    publisher={Elsevier}
  }
```

# Contact

If you have any question, please contact me (He Ziyang) via s210131061@stu.cqupt.edu.cn.
