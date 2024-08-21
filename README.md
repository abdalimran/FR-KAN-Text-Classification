<div align="center">

# Leveraging FourierKAN Classification Head for Pre-Trained Transformer-based Text Classification

</div>

<p align="center">
  <a href="https://imranabdullah.com"><strong>Abdullah Al Imran*</strong></a>
  ·
  <a href="https://farhanishmam.github.io/"><strong>Md Farhan Ishmam*</strong></a>
</p>

<div align="center">

[![arXiv](https://img.shields.io/badge/arXiv-2408.08803-b31b1b.svg?logo=arxiv)](https://arxiv.org/abs/2408.08803) [![arXiv](https://img.shields.io/badge/Code-Repository-blue?logo=GitHub)](https://github.com/abdalimran/FR-KAN-Text-Classification)

</div>

---

We introduce FourierKAN (FR-KAN), a variant of the promising MLP alternative called Kolmogorov-Arnold Networks (KANs), as classification heads for transformer-based encoders. Our studies reveal an average increase of 10% in accuracy and 11% in F1-score when incorporating FR-KAN heads instead of traditional MLP heads for several transformer-based pre-trained models across multiple text classification tasks. FR-KAN heads also train faster and require fewer parameters. 

## Methodology Overview

<img src="assets/method_overview.png" alt="Image Not Found"/>

We propose feature-based fine-tuning of the FR-KAN classification head with different transformer-based pre-trained language models. 

## Performance Evaluation

We evaluated the performance of seven models on seven text classification datasets based on accuracy and F1 score.

<img src="assets/results_full.PNG" alt="Image Not Found" width="800"/>

## Notebooks
- The experiments on every model and dataset can be conducted following the notebooks in `notebooks_experiments`. 
- To conduct ablations on the parameter count of the best-performing models and the impact of grid size, follow the notebooks in `notebooks_ablation`.
- For overall result generation, follow `results.ipynb`.
- To reproduce the visualizations in our work, follow `visualization.ipynb`. 

## Citation

If you find our work useful, please cite our paper:
```
@misc{imran2024leveragingfourierkanclassificationhead,
      title={Leveraging FourierKAN Classification Head for Pre-Trained Transformer-based Text Classification}, 
      author={Abdullah Al Imran and Md Farhan Ishmam},
      year={2024},
      eprint={2408.08803},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2408.08803}, 
}
```

