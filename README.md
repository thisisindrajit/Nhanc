# Using-Deep-CNN-to-enhance-low-res-photos-to-match-the-quality-of-DSLR-cameras
In recent years, there has been a significant improvement in the quality of mobile cameras, bringing mobile photography to a substantially new level. **However, when it comes to artistic quality, mobile devices still fall behind their DSLR counterparts.** To overcome this problem, we present an end-to-end deep learning approach that bridges this gap by translating ordinary low-res photos into DSLR-quality images. **We propose learning the translation function using a deep convolutional neural network that improves both color rendition and image sharpness by taking content, color and texture losses together as the loss function and trying to minimize it.**

## High level block diagram

![image](https://user-images.githubusercontent.com/43838718/108750258-d1172100-7566-11eb-906f-e0d3a4f8d907.png)

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
