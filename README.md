

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


```
Come soon!
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



## Citation

```
Come soon!
```

## License



## Acknowledgement


This implementation is based on [OpenCLIP](https://github.com/mlfoundations/open_clip). Thanks for the awesome work.

## Contact

