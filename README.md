

<h1>CLIP-DINO Spatial Recombination: Enhancing Open-vocabulary Semantic Segmentation without training</h1>


## Come soon!


## Dependencies and Installation


```
git clone https://github.com/yuhao-q/CDSR.git
cd CDSR

conda create -n CDSR python=3.10 -y
conda activate CDSR

pip install -r requirements.txt
```

## Datasets
We include the following dataset configurations in this repo: 
1) `With background class`: PASCAL VOC, PASCAL Context, PASCAL Context 459 (PC459), Cityscapes, ADE20k, ADE847, and COCO-Stuff164k

2) `Without background class`: VOC20, Context59, MaSTr1325, and COCO-Object.

For PASCAL Context 459 and ADE847, please follow the [CAT-Seg](https://github.com/KU-CVLAB/CAT-Seg/tree/main/datasets) to prepare the datasets.
For the other datasets, please follow the [MMSeg data preparation document](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md) to download and pre-process the datasets. 
The COCO-Object dataset can be converted from COCO-Stuff164k by executing the following command:

```
python datasets/cvt_coco_object.py PATH_TO_COCO_STUFF164K -o PATH_TO_COCO164K
```

## Quick Inference
```
python demo.py
```


## Model evaluation
Please modify some settings in `configs/base_config.py` before running the evaluation.




Single-GPU:

```
python eval.py --config ./config/cfg_DATASET.py --workdir YOUR_WORK_DIR
```

Multi-GPU:
```
bash ./dist_test.sh ./config/cfg_DATASET.py
```


## Citation

```
Come soon!
```

## License



## Acknowledgement


This implementation is based on [OpenCLIP](https://github.com/mlfoundations/open_clip) and [ProxyCLIP](https://github.com/mc-lan/ProxyCLIP). Thanks for the awesome work.

## Contact

