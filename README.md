### ContextVLM: Zero-Shot and Few-Shot Context Understanding for Autonomous Driving using Vision Language Models [IEEE ITSC 2024]

This Git Repository contains code for the ContextVLM paper and the associated DrivingContexts dataset. 

In this work, we introduce a dataset called DrivingContexts for the detection of relevant driving contexts for autonomous driving. Additionally, we propose the use of vision language models such as LLaVa and ViLT with zero-shot and few-shot approaches, to solve the problem of detecting such contexts. With our approach, we reduce the need for fully supervised training on large annotated datasets to detect these contexts and also the need for hand-crafted approaches to understand specific contexts of importance.

### Venue

This work is being presented at the [27th IEEE International Conference on Intelligent Transportation Systems (ITSC 2024)](https://ieee-itsc.org/2024/) for the main conference. 

It is also accepted for invited talks at the [Vision and Language Oriented Representation (VALOR)](https://sites.google.com/view/valor-workshop/) workshop and the [Large Language and Vision Models for Autonomous Driving (LLVM-AD)](https://llvm-ad.github.io/)  workshop at ITSC 2024.

### Environment setup
```
pip install -r requirements.txt
```
For installation of LLaVa, the corresponding Notebook- ContextVLM_LLaVA_13b_4bit.ipynb has the relevant steps.

### Dataset

The DrivingContexts dataset is available at https://drive.google.com/drive/folders/1bUNDIlhgTjcxt0WaOGVRRuI0e5_cWJDG.

The dataset has two components - Hand annotated and Machine Annotated. 

The hand annotated component has four subsections, leading to a total of 1,467 images and 35,208 hand annotations for driving contexts.

1. NuScenes
2. KITTI
3. Pittsburgh (Our own data)
4. Web (Data crawled from the Web for uncommon driving contexts)

The machine annotated component has 66,647 images with about 1.6 million multi-VLM annotated driving contexts and only contains data collected by us around Pittsburgh and State College, PA.

### Running Instructions

After downloading the dataset, run the experiments using the associated ipynb notebooks- ContextVLM_LLaVA_13b_4bit.ipynb and ContextVLM_ViLT_finetuning.ipynb.

### Citation

If this work is useful to your research, please kindly recognize our contributions by citing our paper as

```
@misc{sural2024contextvlm,
      title={ContextVLM: Zero-Shot and Few-Shot Context Understanding for Autonomous Driving using Vision Language Models}, 
      author={Shounak Sural and Naren and Ragunathan Rajkumar},
      year={2024},
      eprint={2409.00301},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2409.00301}, 
}
```
