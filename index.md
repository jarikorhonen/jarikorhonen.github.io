## Research Profile

During my research career, I have been working on several different topics, mostly related to multimedia communications and Quality of Experience (QoE). I did my PhD about packet loss resilient audio streaming for Nokia Research Center, Tampere, Finland, during 2001-06. Since 2008, I have been working mostly on visual and audiovisual quality assessment, covering both subjective methodologies and objective quality metrics. You will find some of my recent research highlights with the related resources below.

The list of my publications can be found on [Google Scholar](https://scholar.google.com/citations?hl=en&user=IrbP5FUAAAAJ).


### No-reference video quality assessment

![NR-VQA workflow](https://jarikorhonen.github.io/nr-vqa.png "NR-VQA workflow")

As networks are becoming faster and mobile camera technology more advanced, digital video is all around us. In practice, quality of the video content distributed in the Internet is often impaired by different kinds of distortions, attributed to compression, transmission errors and capture artifacts, such as jerkiness and sensor noise. Subjective quality assessment is often impractical due to the required time and resources. This is why there is need for algorithm-based video quality assessment, known also as *objective video quality metrics*. Objective video quality metrics have several potential applications, such as automatic quality labeling in video distribution services, continuous quality monitoring in streaming systems and user feedback in mobile capture devices, such as tablets and smartphones.

#### Learning-based prediction of packet loss artifact visibility

In QoMEX'18, we have proposed a distortion specific No-Reference Video Quality Metric (NR-VQM) for detecting packet loss artifacts. Unlike most of the other NR-VQMs known in the prior art, the proposed scheme operates at the frame level, not the sequence level, and therefore it can be used to estimate the position of the impacted frames, rather than assessing the sequence level quality only. The metric is based on hand-crafted features and conventional learning-based regression. Since the proposed metric uses distortion-specific features, it is computationally less complex than most general purpose video and image quality metrics.

Implementation of the proposed technique can be downloaded [here](https://github.com/jarikorhonen/nr-vqa-packetloss).

**Reference:**

J. Korhonen, "Learning-based prediction of packet loss artifact visibility in networked video," *IEEE International Conference on Quality of Multimedia Experience (QoMEX'18)*, Sardinia, Italy, May 2018. *(Accepted for publication.)*

### Predicting personal scores for video quality assessment tasks

![Personal scores](https://jarikorhonen.github.io/personal_score.png "Personal scores")

This is basically a simple collaborative filtering scheme that was initially created for predicting missing scores in video quality assessment studies, published in QoMEX'17. The idea was to improve the accuracy of MOS in cases where some users have rated only a subset of items (e.g. video sequences). We assume that this approach could be helpful for reducing the number of participants in quality assessment studies. It could be used also for assessing the reliability of MOS results and possibly also for detecting unreliable test participants.

It should be noted that there are a lot of implementations of different collaborative filtering schemes available (at least if you are ready to switch Matlab to Python), and some other methods may be more efficient for the proposed task than ours. However, to our knowledge, this work is the first one that uses collaborative filtering in visual quality assessment tasks.

Implementation of the method can be downloaded [here](https://github.com/jarikorhonen/personal_scores).

**Reference:**

J. Korhonen, "Predicting personal preferences in subjective video quality assessment," *IEEE International Conference on Quality of Multimedia Experience (QoMEX'17)*, Erfurt, Germany, May 2017. [DOI: 10.1109/QoMEX.2017.7965677](https://doi.org/10.1109/QoMEX.2017.7965677)

### Chroma upsampling for images in Y'CbCr 4:2:0 format

![Chroma upsampling](https://jarikorhonen.github.io/chromaupsample.png "Chroma upsampling")

This is a small piece of work published in ICME'15. Many practical digital images are represented in Y'CbCr 4:2:0 format, where the monochrome version (luma aka Y' component) of the image is coded in higher resolution than the color information (chroma aka Cb and Cr components). When the image is displayed, the resulting RGB image has to be reconstructed by first upsampling the low resolution Cb and Cr images to the same resolution with the Y' component. Since local variations in luma and chroma values are typically correlated, more accurate upsampling results can be obtained by exploiting the luma component in chroma upsampling process.

Matlab implementation for the proposed technique is [here](https://github.com/jarikorhonen/chroma_upsampling).

**Reference:**

J. Korhonen, "Improving image fidelity by luma-assisted chroma subsampling," *IEEE International Conference on Multimedia and Expo (ICME'15)*, Turin, Italy, June 2015. [DOI: 10.1109/ICME.2015.7177387](https://doi.org/10.1109/ICME.2015.7177387)
