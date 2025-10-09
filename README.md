# Awesome-Gradient-Inversion-Attacks

:star: This repository hosts a curated collection of literature associated with **gradient inversion attacks in federated learning**. Feel free to star and fork. For further details, refer to the following paper:

**[Exploring the Vulnerabilities of Federated Learning:
A Deep Dive into Gradient Inversion Attacks](https://pengxin-guo.github.io/FLPrivacy/)** \
[Pengxin Guo](https://pengxin-guo.github.io/)\*, [Runxi Wang](https://scholar.google.com/citations?user=wClrSiMAAAAJ&hl=zh-CN)\*, Shuang Zeng, Jinjing Zhu, Haoning Jiang, Yanran Wang, Yuyin Zhou, Feifei Wang, Hui Xiong, and [Liangqiong Qu](https://liangqiong.github.io/)


## Overview

The existing Gradient Inversion Attacks (GIA) methods can be divided into three types: optimization-based GIA (**OP-GIA**), which works by minimizing the distance between received gradients and gradients computed from dummy data; generation-based GIA (**GEN-GIA**), which utilizes a generator to reconstruct input data; and analytics-based GIA (**ANA-GIA**), which aims to recover input data in closed form. Moreover, GEN-GIA can be further divided into three categories: optimizing the latent vector z, optimizing the generator’s parameters W, and training an inversion generation model. ANA-GIA can be further divided into two categories: manipulating model architecture and manipulating model parameters.

- [Survey Papers](#survey-papers)
- [Optimization-based GIA (OP-GIA)](#optimization-based-gia-op-gia)
- [Generation-based GIA (GEN-GIA)](#generation-based-gia-gen-gia)
  - [Optimizing Latent Vector z](#optimizing-latent-vector-z)
  - [Optimizing Generator's Parameters W](#optimizing-generators-parameters-w)
  - [Training an Inversion Generation Model](#training-an-inversion-generation-model)
- [Analytics-based GIA (ANA-GIA)](#analytics-based-gia-ana-gia)
  - [Manipulating Model Architecture](#manipulating-model-architecture)
  - [Manipulating Model Parameters](#manipulating-model-parameters)
- [Emprical Works](#emprical-works)


## Survey Papers

- **Dealing Doubt: Unveiling Threat Models in Gradient Inversion Attacks under Federated Learning, A Survey and Taxonomy** [[Paper](https://arxiv.org/abs/2405.10376)] \
*Yichuan Shi, Olivera Kotevska, Viktor Reshniak, Abhishek Singh, and Ramesh Raskar* \
arXiv:2405.10376, 2024.

- **The Impact of Adversarial Attacks on Federated Learning: A Survey** [[Paper](https://ieeexplore.ieee.org/document/10274102?denied=)] \
*Kummari Naveen Kumar, Chalavadi Krishna Mohan, and Linga Reddy Cenkeramaddi*\
IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI**), 2023.

- **A Survey on Gradient Inversion: Attacks, Defenses and Future Directions** [[Paper](https://www.ijcai.org/proceedings/2022/0791)] \
*Rui Zhang, Song Guo, Junxiao Wang, Xin Xie, and Dacheng Tao*\
International Joint Conference on Artificial Intelligence (**IJCAI**), 2022.


- **A survey on security and privacy of federated learning** [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0167739X20329848)] \
*Viraaji Mothukuri, Reza M. Parizi, Seyedamin Pouriyeh, Yan Huang, Ali Dehghantanha, and Gautam Srivastava* \
Future Generation Computer Systemsm (**FGCS**), 2021.

## Optimization-based GIA (OP-GIA)

- **Temporal Gradient Inversion Attacks with Robust Optimization** [[Paper](https://ieeexplore.ieee.org/abstract/document/10848255)] \
*Bowen Li, Hanlin Gu, Ruoxin Chen, Jie Li, Chentao Wu, Na Ruan, Xueming Si, and Lixin Fan* \
IEEE Transactions on Dependable and Secure Computing (**TDSC**), 2025.

- **Non-Linear Trajectory Modeling for Multi-Step Gradient Inversion Attacks in Federated Learning** [[Paper](https://arxiv.org/abs/2509.22082)] \
*Li Xia, Zheng Liu, Sili Huang, Wei Tang, and Xuan Liu* \
arXiv:2509.22082, 2025.

- **Boosting Gradient Leakage Attacks: Data Reconstruction in Realistic FL Settings** [[Paper](https://arxiv.org/abs/2506.08435)] \
*Mingyuan Fan, Fuyi Wang, Cen Chen, and Jianying Zhou* \
arXiv:2506.08435, 2025.

- **TS-Inverse: A Gradient Inversion Attack Tailored for Federated Time Series Forecasting Models** [[Paper](https://arxiv.org/abs/2503.20952)] \
*Caspar Meijer, Jiyue Huang, Shreshtha Sharma, Elena Lazovik, and Lydia Y. Chen* \
arXiv:2503.20952, 2025.

- **Gradient Inversion Attacks: Impact Factors Analyses and Privacy Enhancement** [[Paper](https://ieeexplore.ieee.org/abstract/document/10604429)] [[Code](https://github.com/MiLab-HITSZ/2023YeGIAnDe)] \
*Zipeng Ye, Wenjian Luo, Qi Zhou, Zhenqian Zhu, Yuhui Shi, and Yan Jia* \
IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI**), 2024.

- **Hiding in Plain Sight: Disguising Data Stealing Attacks in Federated Learning** [[Paper](https://openreview.net/forum?id=krx55l2A6G)] [[Code](https://github.com/insait-institute/SEER)] \
*Kostadin Garov, Dimitar Iliev Dimitrov, Nikola Jovanović, and Martin Vechev* \
International Conference on Learning Representations (**ICLR**), 2024.

- **Towards Eliminating Hard Label Constraints in Gradient Inversion Attacks** [[Paper](https://openreview.net/forum?id=s8cMuxI5gu)] [[Code](https://github.com/ybwang119/label_recovery)] \
*Yanbo Wang, Jian Liang, Ran He* \
International Conference on Learning Representations (**ICLR**), 2024.

- **GI-SMN: Gradient Inversion Attack Against Federated Learning Without Prior Knowledge** [[Paper](https://link.springer.com/chapter/10.1007/978-981-97-5603-2_36)] \
*Jin Qian, Kaimin Wei, Yongdong Wu, Jilian Zhang, Jinpeng Chen, and Huan Bao* \
International Conference on Intelligent Computing (**ICIC**), 2024.

- **Uncovering Gradient Inversion Risks in Practical Language Model Training** [[Paper](https://dl.acm.org/doi/10.1145/3658644.3690292)] \
*Xinguo Feng, Zhongkui Ma, Zihan Wang, Eu Joe Chegne, Mengyao Ma, Alsharif Abuadbba, and Guangdong Bai* \
ACM Conference on Computer and Communications Security (**CCS**), 2024.

- **Federated Learning under Attack: Improving Gradient Inversion for Batch of Images** [[Paper](https://arxiv.org/abs/2409.17767)] \
*Luiz Leite, Yuri Santo, Bruno L. Dalmazo, and André Riker* \
arXiv:2409.17767, 2024.

- **GI-NAS: Boosting Gradient Inversion Attacks through Adaptive Neural Architecture Search** [[Paper](https://arxiv.org/abs/2405.20725)] \
*Wenbo Yu, Hao Fang, Bin Chen, Xiaohang Sui, Chuan Chen, Hao Wu, Shu-Tao Xia, and Ke Xu* \
arXiv:2405.20725, 2024.

- **AFGI: Towards Accurate and Fast-convergent Gradient Inversion Attack in Federated Learning** [[Paper](https://arxiv.org/abs/2403.08383)] \
*Can Liu, Jin Wang, and Yipeng Zhou, Yachao Yuan, Quanzheng Sheng, and Kejie Lu* \
arXiv:2403.08383, 2024.

- **MGIC: A Multi-Label Gradient Inversion Attack based on Canny Edge Detection on Federated Learning** [[Paper](https://arxiv.org/abs/2403.08284)] \
*Can Liu and Jin Wang* \
arXiv:2403.08284, 2024.

- **Instance-wise Batch Label Restoration via Gradients in Federated Learning** [[Paper](https://openreview.net/forum?id=FIrQfNSOoTr)] [[Code](https://github.com/BUAA-CST/iLRG)] \
*Kailang Ma, Yu Sun, Jian Cui, Dawei Li, Zhenyu Guan, and Jianwei Liu* \
International Conference on Learning Representations (**ICLR**), 2023.

- **Cocktail Party Attack: Breaking Aggregation-Based Privacy in Federated Learning Using Independent Component Analysis** [[Paper](https://proceedings.mlr.press/v202/kariyappa23a.html)] [[Code](https://github.com/facebookresearch/cocktail_party_attack)] \
*Sanjay Kariyappa, Chuan Guo, Kiwan Maeng, Wenjie Xiong, G. Edward Suh, Moinuddin K Qureshi, and Hsien-Hsin S. Lee* \
International Conference on Machine Learning (**ICML**), 2023.

- **Surrogate Model Extension (SME): A Fast and Accurate Weight Update Attack on Federated Learning** [[Paper](https://proceedings.mlr.press/v202/zhu23m.html)] [[Code](https://github.com/JunyiZhu-AI/surrogate_model_extension)] \
*Junyi Zhu, Ruicong Yao, and Matthew B. Blaschko* \
International Conference on Machine Learning (**ICML**), 2023.

- **Gradient Obfuscation Gives a False Sense of Security in Federated Learning** [[Paper](https://www.usenix.org/conference/usenixsecurity23/presentation/yue)] [[Code](https://github.com/KAI-YUE/rog)] \
*Kai Yue, North Carolina State University; Richeng Jin, Zhejiang University; Chau-Wai Wong, Dror Baron, and Huaiyu Dai, and North Carolina State University* \
USENIX Security Symposium (**USENIX Security**), 2023.

- **Data Leakage in Federated Averaging** [[Paper](https://openreview.net/forum?id=e7A0B99zJf)] [[Code](https://github.com/eth-sri/fedavg_leakage)] \
*Dimitar Iliev Dimitrov, Mislav Balunovic, Nikola Konstantinov, and Martin Vechev* \
Transactions on Machine Learning Research (**TMLR**), 2022.

- **GradViT: Gradient Inversion of Vision Transformers** [[Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Hatamizadeh_GradViT_Gradient_Inversion_of_Vision_Transformers_CVPR_2022_paper.html)] \
*Ali Hatamizadeh, Hongxu Yin, Holger R. Roth, Wenqi Li, Jan Kautz, Daguang Xu, and Pavlo Molchanov* \
IEEE/CVF Computer Vision and Pattern Recognition Conference (**CVPR**), 2022.

- **APRIL: Finding the Achilles' Heel on Privacy for Vision Transformers** [[Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Lu_APRIL_Finding_the_Achilles_Heel_on_Privacy_for_Vision_Transformers_CVPR_2022_paper.html)] \
*Jiahao Lu, Xi Sheryl Zhang, Tianli Zhao, Xiangyu He, and Jian Cheng* \
IEEE/CVF Computer Vision and Pattern Recognition Conference (**CVPR**), 2022.

- **CAFE: Catastrophic Data Leakage in Vertical Federated Learning** [[Paper](https://proceedings.neurips.cc/paper_files/paper/2021/hash/08040837089cdf46631a10aca5258e16-Abstract.html)] [[Code](https://github.com/DeRafael/CAFE)] \
*Xiao Jin, Pin-Yu Chen, Chia-Yi Hsu, Chia-Mu Yu, and Tianyi Chen* \
Conference on Neural Information Processing Systems (**NeurIPS**), 2021.

- **See Through Gradients: Image Batch Recovery via GradInversion** [[Paper](https://openaccess.thecvf.com/content/CVPR2021/html/Yin_See_Through_Gradients_Image_Batch_Recovery_via_GradInversion_CVPR_2021_paper.html)] [[Code]()] \
*Hongxu Yin, Arun Mallya, Arash Vahdat, Jose M. Alvarez, Jan Kautz, and Pavlo Molchanov* \
IEEE/CVF Computer Vision and Pattern Recognition Conference (**CVPR**), 2021.

- **Towards General Deep Leakage in Federated Learning** [[Paper](https://arxiv.org/abs/2110.09074)] \
*Jiahui Geng, Yongli Mou, Feifei Li, Qing Li, Oya Beyan, Stefan Decker, and Chunming Rong* \
arXiv:2110.09074, 2021.

- **Inverting Gradients - How easy is it to break privacy in federated learning?** [[Paper](https://proceedings.neurips.cc/paper/2020/hash/c4ede56bbd98819ae6112b20ac6bf145-Abstract.html)] [[Code](https://github.com/JonasGeiping/invertinggradients)] \
*Jonas Geiping, Hartmut Bauermeister, Hannah Dröge, and Michael Moeller* \
Conference on Neural Information Processing Systems (**NeurIPS**), 2020.

- **SAPAG: A Self-Adaptive Privacy Attack From Gradients** [[Paper](https://arxiv.org/abs/2009.06228)] \
*Yijue Wang, Jieren Deng, Dan Guo, Chenghong Wang, Xianrui Meng, Hang Liu, Caiwen Ding, and Sanguthevar Rajasekaran* \
arXiv:2009.06228, 2020.

- **iDLG: Improved Deep Leakage from Gradients** [[Paper](https://arxiv.org/abs/2001.02610)] [[Code](https://github.com/PatrickZH/Improved-Deep-Leakage-from-Gradients)] \
*Bo Zhao, Konda Reddy Mopuri, and Hakan Bilen* \
arXiv:2001.02610, 2020.

- **Deep Leakage from Gradients** [[Paper](https://proceedings.neurips.cc/paper/2019/hash/60a6c4002cc7b29142def8871531281a-Abstract.html)] [[Code](https://github.com/mit-han-lab/dlg)] \
*Ligeng Zhu, Zhijian Liu, and Song Han* \
Conference on Neural Information Processing Systems (**NeurIPS**), 2019.

## Generation-based GIA (GEN-GIA)

### Optimizing Latent Vector z

- **GIFD: A Generative Gradient Inversion Method with Feature Domain Optimization** [[Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Fang_GIFD_A_Generative_Gradient_Inversion_Method_with_Feature_Domain_Optimization_ICCV_2023_paper.html)] [[Code](https://github.com/ffhibnese/GIFD_Gradient_Inversion_Attack)] \
*Hao Fang, Bin Chen, Xuan Wang, Zhi Wang, and Shu-Tao Xia* \
International Conference on Computer Vision (**ICCV**), 2023.

- **Auditing Privacy Defenses in Federated Learning via Generative Gradient Leakage** [[Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Li_Auditing_Privacy_Defenses_in_Federated_Learning_via_Generative_Gradient_Leakage_CVPR_2022_paper.html)] [[Code](https://github.com/zhuohangli/GGL)] \
*Zhuohang Li, Jiaxin Zhang, Luyang Liu, and Jian Liu* \
IEEE/CVF Computer Vision and Pattern Recognition Conference (**CVPR**), 2022.

- **Gradient Inversion with Generative Image Prior** [[Paper](https://proceedings.neurips.cc/paper/2021/hash/fa84632d742f2729dc32ce8cb5d49733-Abstract.html)] [[Code](https://github.com/ml-postech/gradient-inversion-generative-image-prior)] \
*Jinwoo Jeon, jaechang Kim, Kangwook Lee, Sewoong Oh, and Jungseul Ok* \
Conference on Neural Information Processing Systems (**NeurIPS**), 2021.

### Optimizing Generator's Parameters W

- **Generative Image Reconstruction From Gradients** [[Paper](https://ieeexplore.ieee.org/abstract/document/10495167)] \
*Ekanut Sotthiwata, Liangli Zhen, Chi Zhang, Zengxiang Li, and Rick Siow Mong Goh* \
IEEE Transactions on Neural Networks and Learning Systems (**TNNLS**), 2024.

- **Generative Gradient Inversion via Over-Parameterized Networks in Federated Learning** [[Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_Generative_Gradient_Inversion_via_Over-Parameterized_Networks_in_Federated_Learning_ICCV_2023_paper.html)] [[Code](https://github.com/czhang024/CI-Net)] \
*Chi Zhang, Zhang Xiaoman, Ekanut Sotthiwat, Yanyu Xu, Ping Liu, Liangli Zhen, and Yong Liu* \
International Conference on Computer Vision (**ICCV**), 2023.

- **GRNN: Generative Regression Neural Network—A Data Leakage Attack for Federated Learning** [[Paper](https://dl.acm.org/doi/abs/10.1145/3510032)] [[Code](https://github.com/Rand2AI/GRNN)] \
*Hanchi Ren, Jingjing Deng, and Xianghua Xie* \
ACM Transactions on Intelligent Systems and Technology (**TIST**), 2022.

### Training an Inversion Generation Model

- **Fast Generation-Based Gradient Leakage Attacks against Highly Compressed Gradients** [[Paper](https://ieeexplore.ieee.org/abstract/document/10229091)] [[Code](https://github.com/pigeon-dove/FGLA)] \
*Dongyun Xue, Haomiao Yang, Mengyu Ge, Jingwei Li, Guowen Xu, and Hongwei Li* \
IEEE International Conference on Computer Communications (**INFOCOM**), 2023.

- **Learning To Invert: Simple Adaptive Attacks for Gradient Inversion in Federated Learning** [[Paper](https://proceedings.mlr.press/v216/wu23a.html)] [[Code](https://github.com/wrh14/Learning_to_Invert)] \
*Ruihan Wu, Xiangyu Chen, Chuan Guo, and Kilian Q. Weinberger*\
Conference on Uncertainty in Artificial Intelligence (**UAI**), 2023.

## Analytics-based GIA (ANA-GIA)

### Manipulating Model Architecture

- **Loki: Large-scale Data Reconstruction Attack against Federated Learning through Model Manipulation** [[Paper](https://ieeexplore.ieee.org/abstract/document/10646724)] [[Code](https://github.com/Manishpandey-0/Adversarial-reconstruction-attack-on-FL-using-LOKI)] \
*Joshua C. Zhao, Atul Sharma, Ahmed Roushdy Elkordy, Yahya H. Ezzeldin, Salman Avestimehr, and Saurabh Bagchi* \
IEEE Symposium on Security and Privacy (**S&P**), 2024.


- **Robbing the Fed: Directly Obtaining Private Data in Federated Learning with Modified Models** [[Paper](https://openreview.net/forum?id=fwzUgo0FM9v&ref=morioh.com&utm_source=morioh.com)] [[Code](https://github.com/lhfowl/robbing_the_fed)] \
*Liam H Fowl, Jonas Geiping, Wojciech Czaja, Micah Goldblum, and Tom Goldstein* \
International Conference on Learning Representations (**ICLR**), 2022.

### Manipulating Model Parameters

- **Gradient Inversion Attacks on Parameter-Efficient Fine-Tuning** [[Paper](https://openaccess.thecvf.com/content/CVPR2025/html/Sami_Gradient_Inversion_Attacks_on_Parameter-Efficient_Fine-Tuning_CVPR_2025_paper.html)] [[Code](https://github.com/info-ucr/PEFTLeak)] \
*Hasin Us Sami, Swapneel Sen, Amit K. Roy-Chowdhury, Srikanth V. Krishnamurthy, and Basak Guler* \
IEEE/CVF Computer Vision and Pattern Recognition Conference (**CVPR**), 2025.

- **Maximum Knowledge Orthogonality Reconstruction With Gradients in Federated Learning** [[Paper](https://openaccess.thecvf.com/content/WACV2024/html/Wang_Maximum_Knowledge_Orthogonality_Reconstruction_With_Gradients_in_Federated_Learning_WACV_2024_paper.html)] [[Code](https://github.com/wfwf10/MKOR)] \
*Feng Wang, Senem Velipasalar, and M. Cenk Gursoy* \
Winter Conference on Applications of Computer Vision (**WACV**), 2024.

- **When the Curious Abandon Honesty: Federated Learning Is Not Private** [[Paper](https://ieeexplore.ieee.org/abstract/document/10190537)] \
*Franziska Boenisch, Adam Dziedzic, Roei Schuster, Ali Shahin Shamsabadi, Ilia Shumailov, and Nicolas Papernot* \
IEEE European Symposium on Security and Privacy (**EuroS&P**), 2023.

- **Fishing for User Data in Large-Batch Federated Learning via Gradient Magnification** [[Paper](https://proceedings.mlr.press/v162/wen22a.html)] \
*Yuxin Wen, Jonas A. Geiping, Liam Fowl, Micah Goldblum, and Tom Goldstein* \
International Conference on Machine Learning (**ICML**), 2022.

- **Eluding Secure Aggregation in Federated Learning via Model Inconsistency** [[Paper](https://dl.acm.org/doi/abs/10.1145/3548606.3560557)] [[Code](https://github.com/pasquini-dario/EludingSecureAggregation)] \
*Dario Pasquini, Danilo Francati, and Giuseppe Ateniese* \
ACM SIGSAC Conference on Computer and Communications Security (**CCS**), 2022.

## Emprical Works

- **SoK: On Gradient Leakage in Federated Learning** [[Paper](https://arxiv.org/abs/2404.05403)] \
*Jiacheng Du, Jiahui Hu, Zhibo Wang, Peng Sun, Neil Zhenqiang Gong, Kui Ren, and Chun Chen* \
USENIX Security Symposium (**USENIX Security**), 2025.

- **Hear No Evil: Detecting Gradient Leakage by Malicious Servers in Federated Learning** [[Paper](https://arxiv.org/abs/2506.20651)] \
*Fei Wang and Baochun Li* \
arXiv:2506.20651, 2025.

- **FEDLAD: Federated Evaluation of Deep Leakage Attacks and Defenses** [[Paper](https://arxiv.org/abs/2411.03019)] \
*Isaac Baglin, Xiatian Zhu, and Simon Hadfield* \
arXiv:2411.03019, 2024.

- **Evaluating Gradient Inversion Attacks and Defenses in Federated Learning** [[Paper](https://proceedings.neurips.cc/paper/2021/hash/3b3fff6463464959dcd1b68d0320f781-Abstract.html)] [[Code](https://github.com/Princeton-SysML/GradAttack)] \
*Yangsibo Huang, Samyak Gupta, Zhao Song, Kai Li, and Sanjeev Arora* \
Conference on Neural Information Processing Systems (**NeurIPS**), 2021.