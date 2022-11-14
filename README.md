# aiMotive Multimodal Dataset
Autonomous driving is a popular research area within the computer vision research community.  Since autonomous vehicles are highly safety-critical, ensuring robustness is essential for real-world deployment. While several public multimodal datasets are accessible, they mainly comprise two sensor modalities (camera, LiDAR) which are not well suited for adverse weather. In addition, they lack far-range annotations, making it harder to train neural networks that are the base of a highway assistant function of an autonomous vehicle. Therefore, we introduce a multimodal dataset for robust autonomous driving with long-range perception. The dataset consists of 176 scenes with synchronized and calibrated LiDAR, camera, and radar sensors covering a 360-degree field of view. The collected data was captured in highway, urban, and suburban areas during daytime, night, and rain and is annotated with 3D bounding boxes with consistent identifiers across frames. Furthermore, we trained unimodal and multimodal baseline models for 3D object detection.

### Download
The full dataset (~85 GB) can be downloaded from this [link](https://aimotive-dataset.s3.eu-central-1.amazonaws.com/aimotive-dataset.zip).

### Dataset loader and renderer
A dataset renderer and a PyTorch data loader example can be found in this [repository](https://github.com/aimotive/aimotive-dataset-loader).

### Multimodal model training repository
Our training repository built on the top of [BEVDepth](https://github.com/Megvii-BaseDetection/BEVDepth) can be found [here](https://github.com/aimotive/mm_training).

## Cite our work
If you use this code or aiMotive Multimodal Dataset in your research, please cite our work by using the following BibTeX entry:

```latex
 @article{matuszka2022aimotivedataset,
  title={aiMotive Dataset: A Multimodal Dataset for Robust Autonomous Driving with Long-Range Perception},
  author={Matuszka, Tamás and Németh, Gabor and Varga, Bálint and Kunsági-Máté, Sándor and Barton, Iván and Hajas, Péter and Szeghy, Dávid and Pető, Levente},
  journal={arXiv preprint arXiv:XXXXXXXX},
  year={2022}
}
```
