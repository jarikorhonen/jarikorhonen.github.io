## Research Profile

During my research career, I have been working on several different topics, mostly related to multimedia communications and Quality of Experience (QoE). I did my PhD about packet loss resilient audio streaming for Nokia Research Center, Tampere, Finland, during 2001-06. Since 2008, I have been working mostly on visual and audiovisual quality assessment, covering both subjective methodologies and objective quality metrics.

The list of my publications can be found on [Google Scholar](https://scholar.google.com/citations?hl=en&user=IrbP5FUAAAAJ).

### Upsampling of images in Y'CbCr 4:2:0 format

This is a small piece of work published in ICME'15. Many practical digital images are represented in Y'CbCr 4:2:0 format, where the monochrome version (luma aka Y' component) of the image is coded in higher resolution than the color information (chroma aka Cb and Cr components). When the image is displayed, the resulting RGB image has to be reconstructed by first upsampling the low resolution Cb and Cr images to the same resolution with the Y' component. Since local variations in luma and chroma values are typically correlated, more accurate upsampling results can be obtained by exploiting the luma component in chroma upsampling process.

Matlab implementation for the proposed technique can be found here.

Reference: J. Korhonen, "Improving image fidelity by luma-assisted chroma subsampling," *IEEE International Conference on Multimedia and Expo (ICME'15)*, Turin, Italy, June 2015. [DOI: 10.1109/ICME.2015.7177387](https://ieeexplore.ieee.org/document/7177387/)
