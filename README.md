# SRVC-LA: Sparse regularization of visual context and latent attention based model for video description

Pengjie Tang, Jiayu Zhang, Hanli Wang, Yunlan Tan, Yun Yi

Code of Neurocomputing 2025 paper [SRVC-LA: Sparse regularization of visual context and latent attention based model for video description](https://www.sciencedirect.com/science/article/abs/pii/S092523122500311X)

### ABSTRACT

Video description is one of the important generative tasks, which is to summarize the visual content and translate it into natural language. Nowadays, an increasing number of effective models have been developed for this task. Nevertheless, the visual and language features are combined and represented in a dense multimodal feature space in popular works, making it easy for the model to become stuck in over fitting. This results in the model lacking sufficient generalization ability. A model with sparse regularization of visual context and latent attention (SRVC-LA) is proposed in this work. According to encoding padding sequence corresponding to the encoded video and then concatenation of visual contextual features, the visual regularization context is extracted for vision attention sparsity. Then it is attended by a latent attention mechanism, where the visual regularization context and the previous hidden state is combined and attended for multi-modal semantic alignment. Additionally, the visual and language features are combined with their respective latent attention features and fed to two branches for semantic compensation. Experiments on MSVD and MSR-VTT2016 datasets are conducted, and better performances are achieved compared to the baseline and other popular models,demonstrating the effectiveness and superiority of the proposed model.

## How to run

### Training

```
$ python train.py
```

### testing

```
$ python eval.py
```

### Requirements

We have simple requirements:
The main requirements are:

```
python > 3.1
pytorch > 1.6
```

Other python packages: nltk, pycocotools, pyyaml, easydict, datasets, boto3, ftfy, regex, tqdm

### Datasets

Due to copyright issue, we could not release the raw videos. We suggest downloading the orignal raw videos from the official dataset websites.

Please refer to [this repo](https://github.com/openai/CLIP) for extracting the CLIP features (ViT-B-32).

### Reference

If you find this repository useful, please consider citing our work:

```
@article{tang2025srvc,
  title={SRVC-LA: Sparse regularization of visual context and latent attention based model for video description},
  author={Tang, Pengjie and Zhang, Jiayu and Wang, Hanli and Tan, Yunlan and Yi, Yun},
  journal={Neurocomputing},
  pages={129639},
  year={2025},
  publisher={Elsevier}
}
```
