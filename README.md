# MFQEv2 dataset

## Background

A lossless YUV video dataset provided by MFQEv2, including:

- 108 lossless YUV videos for training.
- 18 lossless YUV videos for test, recommended by ITU-T.
- An HEVC compression tool box (HM16.5, LDP, QP37).

For more details, please refer to our paper.

## Data unzip and compression

First edit `option.yml` in `video_compression/`, i.e., `dir_dataset` and `qp`.

Then run:

```bash
$ cd video_compression/
$ chmod +x TAppEncoderStatic
$ python unzip_n_compress.py
```

Finally, we will get:

```tex
MFQEv2_dataset/
├── train_108/
│   ├── raw/
│   └── HM16.5_LDP/
│       └── QP37/
├── test_18/
│   ├── raw/
│   └── HM16.5_LDP/
│       └── QP37/
├── video_compression/
│   └── ...
└── README.md
```

## Citation

If you find this helpful, you may cite：

@ARTICLE{MFQEv2,
author={Z. {Guan} and Q. {Xing} and M. {Xu} and R. {Yang} and T. {Liu} and Z. {Wang}},
journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
title={{MFQE} 2.0: A New Approach for Multi-frame Quality Enhancement on Compressed Video},
year={2019},
volume={},
number={},
pages={1-1},
keywords={Quality enhancement;compressed video;deep learning},
doi={10.1109/TPAMI.2019.2944806},
ISSN={},
month={},
}
