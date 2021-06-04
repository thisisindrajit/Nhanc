# Nhanc - Enhance your low resolution images to DSLR quality levels using Deep Learning
In recent years, there has been a significant improvement in the quality of mobile cameras, bringing mobile photography to a substantially new level. **However, when it comes to artistic quality, mobile devices still fall behind their DSLR counterparts.** To overcome this problem, we present an end-to-end deep learning approach that bridges this gap by translating ordinary low-res photos into DSLR-quality images. **We propose learning the translation function using a deep convolutional neural network that improves both color rendition and image sharpness by taking content, color and texture losses together as the loss function and trying to minimize it.**

## High level block diagram

![image](https://user-images.githubusercontent.com/43838718/108750258-d1172100-7566-11eb-906f-e0d3a4f8d907.png)

## Dataset

A smaller version of the original DPED dataset was used. 

Link to the dataset - https://drive.google.com/drive/folders/1x5-JNsSG0XA0SelKrkBd6w5S_6G6huYk?usp=sharing

## Model Log

After training the model primarily on iPhone images for 10000 iterations, the log obtained is as follows:

| Type | Metrics |
| ---- | ---- |
| discriminator accuracy | train: 0.537, test: 0.5386 |
| generator losses | content: 7.315, color: 108.8, texture: -34.45, total variation: 0.00247 |
| General | psnr: 20.23, ms-ssim: 0.9161 |

## Visual Results

![predict_1_before_after](https://user-images.githubusercontent.com/43838718/115104326-50c4d900-9f75-11eb-8a12-825847d42123.png)
![predict_5_before_after](https://user-images.githubusercontent.com/43838718/115104329-54586000-9f75-11eb-94a3-341edd47732f.png)
![predict_6_before_after](https://user-images.githubusercontent.com/43838718/115104331-56222380-9f75-11eb-9670-9e242d87f2ce.png)
![predict_11_before_after](https://user-images.githubusercontent.com/43838718/115104334-57ebe700-9f75-11eb-8f32-c8fdde319dfd.png)

## Reference

This notebook contains references for code from this repository: https://github.com/aiff22/DPED.git

This project is for educational purposes only.

## Citation:

<pre>
@inproceedings{ignatov2017dslr,
  title={DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks},
  author={Ignatov, Andrey and Kobyshev, Nikolay and Timofte, Radu and Vanhoey, Kenneth and Van Gool, Luc},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision},
  pages={3277--3285},
  year={2017}
}
</pre>
