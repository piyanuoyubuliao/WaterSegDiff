## Thank you for your interest in WaterSegDiff: A Dual Constraint-Controlled Diffusion Model for Synchronous Generation of Underwater Images and Semantic Masks.

## 🔬 Paper Information

This work has been submitted as a Regular Paper to IEEE Transactions on Circuits and Systems for Video Technology (TCSVT).

WaterSegDiff addresses a fundamental bottleneck in underwater semantic segmentation: the scarcity of high-quality, manually annotated underwater datasets.

To tackle this issue, we propose a dual-controlled diffusion framework for the synchronous generation of high-fidelity underwater images and aligned semantic masks. The model is designed to maintain strong structural integrity and semantic consistency between generated image–mask pairs, which is critical for downstream perception tasks.

## 🚀 Key Contributions

🔹**Dual-Controlled Diffusion Framework**

A deeply coupled architecture that ensures sub-pixel alignment between images and masks, mitigating semantic drift during generation.

🔹**Structural Constraint via HED Priors**

Incorporation of Holistically-Nested Edge Detection (HED) maps as structural guidance, overcoming the spatial limitations of text-only conditioning.

🔹**Specialized Mask Adapter**

A mask-aware refinement module bridging the gap between discrete semantic labels and continuous latent representations.

🔹**Large-Scale Synthetic Dataset**

We synthesized 24,957 high-quality underwater image–mask pairs. Experimental results on USIS10K and UIIS demonstrate significant segmentation improvements when training with our generated data.

## 🚧 Full source code and complete dataset will be publicly released after the paper is officially accepted.

## 📌 Current Status

At this stage, we provide:

🔹 Results of Quantitative Comparison Experiments

### 📊 USIS10K
| Method | Generation Model | mIou↑ |	aAcc↑ |	mAcc↑ |	mDice↑ |	mFscore↑ |	mPrecision↑ |	mRecall↑ |
|:------:|:----------------:|:------:|:-------:|:-------:|:--------:|:---------:|:------------:|:----------:|
|SegMAN|TIDE (CVPR2025)|73.81|**81.36**|**89.07**|84.83|84.83|81.23|**89.07**|
|SegMAN|[WaterSegDiff (Ours)](https://drive.google.com/file/d/18swPtK8kcJ70HTUNzHlZ1JywZ6SKqiCM/view?usp=sharing)|**74.66**|77.78|86.45|**85.32**|**85.32**|**84.61**|86.45|
|Mask2Former|TIDE (CVPR2025)|71.17|87.76|85.26|83.09|83.09|82.40|85.26|
|Mask2Former|[WaterSegDiff (Ours)](https://drive.google.com/file/d/1cIYERgSTdI0iI5w45WffpGFwlhGsH7uI/view?usp=sharing)|**72.82**|**88.86**|**86.69**|**84.23**|**84.23**|**83.33**|**86.69**|

### 📊 UIIS
| Method | Generation Model | mIou↑ |	aAcc↑ |	mAcc↑ |	mDice↑ |	mFscore↑ |	mPrecision↑ |	mRecall↑ |
|:------:|:----------------:|:------:|:-------:|:-------:|:--------:|:---------:|:------------:|:----------:|
|SegMAN|TIDE (CVPR2025)|67.33|73.83|84.26|79.63|79.63|76.52|84.26|
|SegMAN|[WaterSegDiff (Ours)](https://drive.google.com/file/d/1KuH0tm3Jt32vrUzHu_jZ8Y_Ve8JJUW8O/view?usp=sharing)|**71.65**|**74.17**|**88.85**|**83.35**|**83.35**|**79.17**|**88.85**|
|Mask2Former|TIDE (CVPR2025)|61.13|89.63|79.47|73.10|73.10|70.03|79.47|
|Mask2Former|[WaterSegDiff (Ours)](https://drive.google.com/file/d/1srpiqvO_m0jqL5T4f8y8pBjTw3uPl2uI/view?usp=sharing)|**69.43**|**93.15**|**89.62**|**81.26**|**81.26**|**76.11**|**89.62**|

🔹 Example generated image–mask pairs

[**WaterSegDiff Example pairs**](assets/WSDSample.zip)

More materials will be continuously updated.

## 🌊 What WaterSegDiff Will Provide

WaterSegDiff is designed to synchronously generate high-quality underwater image–semantic mask pairs under dual constraint control.

After release, users will be able to:

### 1️⃣ Generate Custom Image–Mask Pairs

Use our diffusion framework to:

🔹 Generate large-scale underwater image–mask pairs

🔹 Control semantic structures during generation

🔹 Train the model on your own underwater datasets

### 2️⃣ Directly Use Our Pre-generated Dataset

We will also provide:

🔹 A large-scale synthetic underwater image–mask paired dataset

🔹 Ready-to-use training format

This allows researchers to directly train  models without additional generation steps.

## 📬 Stay Tuned

If you are interested in collaboration or early access, feel free to contact us.

⭐ Please star this repository to stay updated with the official release!
