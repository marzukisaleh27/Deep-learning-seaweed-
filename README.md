# Deep-learning-seaweed-
## Spectral-Spatial UNet for mapping seaweed cultivation
Spectral-Spatial UNet (SSUNet) model for seaweed cultivation mapping. The architecture of SSUNet is composed of several layers of convolution, up-convoultion, pooling, and attention. Here we try to add a combination of spectral attention and spatial attention modules (SSAM) in each UNet layer. In detail, you can see the following figure:

![SSUNet_seaweed_new_upfont](https://github.com/user-attachments/assets/bcf74da8-00c5-48b0-95a1-d959a873b52a)

The model was built using remote sensing data, namely PlanetScope imagery. Several preprocessing treatments were applied to the dataset prior to label data generation. The label collection process applies the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything).

The training model results show good accuracy. The inference model can be shown as follows. There are still some prediction results that show false negative and false positive. <br/>
<img src="https://github.com/user-attachments/assets/e0229dc7-7321-487a-9698-9d5f367d6a19" alt="compare" width="50%" height="50%">

The results of this research are described in detail in [this paper](https://so04.tci-thaijo.org/index.php/MTR/article/view/273926). If you want to try model inference, you can use [the trained model](https://drive.google.com/file/d/1hqJbixpFMVNknsIF35gQDHsI2Ec7tKnE/view?usp=drive_link) with your dataset. See the [Predict](./Script/Predict.ipynb) code file for details. But first, make sure your dataset matches the configuration desired by the model.

This research is also part of the development of a deep learning model for seaweed cultivation mapping conducted by KONEKSI. View [Seaweed-Koneksi](https://github.com/KoneksiSeaweed/Seaweed-Koneksi)

## License
Access to Planet data is restricted. View [Terms of Use](https://www.planet.com/terms-of-use/).

## Contact
[email](mailto:marzuki1999@mail.ugm.ac.id)

## How to cite
Bibtex:
```
@article{Marzuki2025,
  title={Spectral-Spatial Deep Learning Model for Seaweed Cultivation Mapping Using PlanetScope Imagery in Pangkajene and Islands Regency},
  author={Marzuki and Arjasakusuma, Sanjiwana and Khakhim, Nurul and Wicaksono, Pramaditya and Farda, Nur Mohammad and Utami, Nur Laila Eka},
  journal={Maritime Technology and Research},
  volume={7},
  number={2},
  pages={1--10},
  year={2025},
  doi={10.33175/mtr.2025.273926}
}
```

## Acknowledgements
This publication has been funded by the Department of Foreign Affairs and Trade Australia through KONEKSI. The views expressed in this publication are the authors’ alone and are not necessarily the views of the Australian Government.
