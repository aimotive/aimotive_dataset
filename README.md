# aiMotive Multimodal Dataset
Autonomous driving is a popular research area within the computer vision research community.  Since autonomous vehicles are highly safety-critical, ensuring robustness is essential for real-world deployment. While several public multimodal datasets are accessible, they mainly comprise two sensor modalities (camera, LiDAR) which are not well suited for adverse weather. In addition, they lack far-range annotations, making it harder to train neural networks that are the base of a highway assistant function of an autonomous vehicle. Therefore, we introduce a multimodal dataset for robust autonomous driving with long-range perception. The dataset consists of 176 scenes with synchronized and calibrated LiDAR, camera, and radar sensors covering a 360-degree field of view. The collected data was captured in highway, urban, and suburban areas during daytime, night, and rain and is annotated with 3D bounding boxes with consistent identifiers across frames. Furthermore, we trained unimodal and multimodal baseline models for 3D object detection.

You can read the paper about the dataset [here](https://arxiv.org/abs/2211.09445).

### Download
The dataset is made freely available for non-commercial research purposes only. The full dataset (~85 GB) can be downloaded by filling this [form](https://forms.gle/rHW75TSEQJQhQ1Bm6).

[Kaggle](https://www.kaggle.com/datasets/tamasmatuszka/aimotive-multimodal-dataset) provides an alternative option for using the dataset.

### Dataset loader and renderer
A dataset renderer and a PyTorch data loader example can be found in this [repository](https://github.com/aimotive/aimotive-dataset-loader).

### Multimodal model training repository
Our training repository built on the top of [BEVDepth](https://github.com/Megvii-BaseDetection/BEVDepth) can be found [here](https://github.com/aimotive/mm_training).

## Cite our work
If you use this code or aiMotive Multimodal Dataset in your research, please cite our [work](https://arxiv.org/abs/2211.09445) by using the following BibTeX entry:

```latex
 @article{matuszka2022aimotivedataset,
  title = {aiMotive Dataset: A Multimodal Dataset for Robust Autonomous Driving with Long-Range Perception},
  author = {Matuszka, Tamás and Barton, Iván and Butykai, Ádám and Hajas, Péter and Kiss, Dávid and Kovács, Domonkos and Kunsági-Máté, Sándor and Lengyel, Péter and Németh, Gábor and Pető, Levente and Ribli, Dezső and Szeghy, Dávid and Vajna, Szabolcs and Varga, Bálint},
  doi = {10.48550/ARXIV.2211.09445},
  url = {https://arxiv.org/abs/2211.09445},
  publisher = {arXiv},
  year = {2022},
}
```
