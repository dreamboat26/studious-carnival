# Comparative Study of Machine Unlearning Techniques for Computer Vision and NLP Models

<div align="center">
  <img src="https://github.com/user-attachments/assets/8acdaa6a-6609-496c-8729-a46192f89e87" alt="snip2">
</div>

This repository contains the code, datasets, results, and supplementary materials associated with the paper **"Comparative Study of Machine Unlearning Techniques for Computer Vision and NLP Models"** by **Mahule Roy**.

---

## Abstract

Machine unlearning is a critical field in machine learning aimed at efficiently removing specific data's influence on trained models. This capability is essential for compliance with data privacy regulations, correcting erroneous data, and adapting models to evolving datasets. This study explores unlearning methods in computer vision using CIFAR-10 and CIFAR-100 datasets and in NLP with biased medical datasets. Techniques like neural masking, retraining, instruction fine-tuning, and knowledge distillation were implemented to evaluate unlearning performance while maintaining overall model accuracy. The results highlight the effectiveness of these techniques in balancing privacy and performance.

---

## Repository Contents

### 1. **Paper**
- A PDF copy of the full research paper is available in the `docs/` folder.

### 2. **Code**
- Scripts and implementations for:
  - **Computer Vision Tasks**:
    - Neural masking on VGG16.
    - Retraining on retain sets for ResNet18, EfficientFormerV2, and CoAtNet.
    - Knowledge distillation using competent and incompetent teacher models.
  - **NLP Tasks**:
    - Instruction fine-tuning of LLaMA models using biased datasets.
    - Prompt engineering for bias unlearning.

### 3. **Data**
- The repository includes preprocessing scripts and references to public datasets:
  - **CIFAR-10 and CIFAR-100**: For computer vision tasks.
  - **Medical Biased Dataset**: From Huggingface for NLP tasks.

### 4. **Results**
- Visualizations of metrics such as accuracy, precision, recall, and F1-score for baseline and unlearned models.
- Screenshots of outputs for NLP tasks using LLaMA models.

---

## Key Features

1. **Neural Masking**:
   - Applied to VGG16 for targeted unlearning in computer vision.
   - Demonstrates selective forgetting with minimal impact on other classes.

2. **Knowledge Distillation**:
   - Implemented with dual-teacher models (competent and incompetent teachers).
   - Optimized unlearning without full retraining.

3. **Instruction Fine-Tuning**:
   - Used for bias unlearning in LLaMA models.
   - Achieves effective unlearning with reduced computational overhead.

4. **Evaluation Metrics**:
   - Includes metrics like KL divergence, ZRF scores, and accuracy on retain and forget sets.

---

## How to Use

### Prerequisites
- Python 3.8+ and a compatible GPU environment.
- Clone this reporsitory:
  ```bash
  git clone https://github.com/dreamboat26/studious-carnival.git
  cd studious-carnival
  ```
- Run Experiments based on the seperate .ipynb files added
- Visualize the results

## Citation

If you use this repository or reference this work, please cite it as follows:

```bibtex
@article{mahule2025unlearning,
  title={Comparative Study of Machine Unlearning Techniques for Computer Vision and NLP Models},
  author={Mahule, Roy},
  conference={International Conference on Machine Learning and Human-Computer Interaction},
  year={2025},
  doi={10.13140/RG.2.2.13752.87049},
  url={https://paperswithcode.com/paper/comparative-study-of-machine-unlearning}
}
```

## Acknowledgements

I would like to thank the open source community and the Arxiv papers which have been a huge help in drafting this paper and proceeding with my implementations.

## License

This paper is licensed under MIT Lincense.


