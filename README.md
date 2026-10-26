# BanTrafficNet: Bangladeshi Traffic Sign Recognition

[![Paper](https://img.shields.io/badge/Scientific%20Reports-10.1038%2Fs41598--025--33038--y-blue)](https://doi.org/10.1038/s41598-025-33038-y)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)

Official code and dataset release for:

> **Bangladeshi traffic sign recognition using the lightweight BanTrafficNet deep learning approach**
> Md Mahbubur Rahman Tusher, Fahmid Al Farid, Hasan Muhammad Kafi, Abu Saleh Musa Miah, Susmita Roy Rinky, Muhiminul Islam, Md. Abdur Rahim, Sarina Mansor, Hezerul Abdul Karim
> *Scientific Reports* 16, 31000 (2026). https://doi.org/10.1038/s41598-025-33038-y

## About

Traffic sign recognition is a key part of driver-assistance and intelligent transportation systems, but Bangladeshi road signs have been largely overlooked because no public dataset existed for them. This repository fills that gap.

It contains:

- **BDTSR** – the Bangladesh Traffic Sign Recognition dataset: 48 classes of regulatory, warning and information signs photographed on real roads across Bangladesh (6,417 original images, 24,000 after augmentation).
- **BanTrafficNet** – a lightweight CNN (~4.6M parameters) trained to classify these signs, small enough to run on a phone.
- Code to train and evaluate the model on BDTSR as well as the GTSRB (Germany) and BTSC (Belgium) benchmarks.

BanTrafficNet reaches **99.34%** test accuracy on BDTSR, 96.97% on GTSRB and 98.82% on BTSC, and has been validated in the field through an Android app running the model via TensorFlow Lite.

## Dataset

BDTSR images are organised by class ID, with a mapping file from ID to sign name. Signs include speed limits, no overtaking, no U-turn, give way, Y-junction, railway crossing, mosque, hospital, bus stop and more.

### Sample images

<p align="center">
  <img src="traffic%20sign%20recognition/Bangladesh/Dataset/Final_BDTSR/BDTSR/train/00001/10000000000000.jpg" width="140" alt="BDTSR class 00001"/>
  <img src="traffic%20sign%20recognition/Bangladesh/Dataset/Final_BDTSR/BDTSR/train/00006/100.jpg" width="140" alt="BDTSR class 00002"/>
  <img src="traffic%20sign%20recognition/Bangladesh/Dataset/Final_BDTSR/BDTSR/train/00010/1.jpg" width="140" alt="BDTSR class 00003"/>
  <img src="traffic%20sign%20recognition/Bangladesh/Dataset/Final_BDTSR/BDTSR/train/00019/10.jpg" width="140" alt="BDTSR class 00004"/>
  <img src="traffic%20sign%20recognition/Bangladesh/Dataset/Final_BDTSR/BDTSR/train/00044/1.jpg" width="140" alt="BDTSR class 00005"/>
</p>

GTSRB and BTSC are redistributed here for convenience. Official sources:

- GTSRB – https://benchmark.ini.rub.de/gtsrb_news.html
- BTSC – https://btsd.ethz.ch/shareddata/

## Getting Started

```bash
git clone https://github.com/tusher100/Traffic_Sign_Recognition.git
cd Traffic_Sign_Recognition
pip install -r requirements.txt
```

Download and extract the dataset into the `data/` folder, then open the notebook for the dataset you want to work with and run the cells in order. The notebooks cover data loading, augmentation, training, evaluation and exporting the model.

## Citation

If you use the BDTSR dataset or BanTrafficNet in your research, please cite:

```bibtex
@article{tusher2026bangladeshi,
  title={Bangladeshi traffic sign recognition using the lightweight BanTrafficNet deep learning approach},
  author={Tusher, Md Mahbubur Rahman and Farid, Fahmid Al and Kafi, Hasan Muhammad and Miah, Abu Saleh Musa and Rinky, Susmita Roy and Islam, Muhiminul and Rahim, Md Abdur and Mansor, Sarina and Karim, Hezerul Abdul},
  journal={Scientific Reports},
  volume={16},
  number={1},
  pages={31000},
  year={2026},
  publisher={Nature Publishing Group UK, London}
}
```

## License

Released under the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). GTSRB and BTSC remain subject to their original licenses.

## Contact

**Md Mahbubur Rahman Tusher**
mdmahbuburrahmantusher@gmail.com
