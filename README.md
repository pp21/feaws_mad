# Database for face morphing attack detection and localization based on feature-wise supervision

## Introduction

The morphed face images database (henceforth, ''database'') contains images used for the detection of face morphing attacks. To foster the research of face morphing attack detection, the database will be released to researchers for academic research purpose upon request.

The database is developed based on the face images from the public [ND-IIITD database](https://ieeexplore.ieee.org/document/7464282) and [the self-collected face images](https://github.com/pp21/watchlist-MAD). Unfortunately, due to the restriction of ND-IIITD database's release agreement, this part may not be released. But like the previously published paper, the list of the face image pairs used for morph generation will be released. For the part developed based on the self-collected face images, it will be fully released to the research community upon request.

The database is summarized below.

| Number of images         | complete | splicing | retouching | combined |
| :--:                     | :--:     | :--:     | :--:       | :--:     |
| Training (ND-IIITD)      | 1050     | 1050     | 1050       | 1050     |
| Testing (ND-IIITD)       | 223      | 158      | 231        | 208      |
| Testing (self-collected) | 3675     | 3788     | 3387       | 3819     |

Some images of the database are shown below, the black boxes are used for privacy concerns but are not used in the experiments. (a) Bona fide image 1. (b) Complete morphed image [1]. (c) Splicing morphed image [1]. (d) Retouching morphed image [2]. (e) Combined morphed image [3]. (f) Bona fide image 2. The morphing weight is 0.5.

<div align="center">
  <img src="https://github.com/pp21/feaws_mad/blob/main/images.jpg">
</div>

## Testing protocols

The database contains 5 testing protocols with the the variations of morphing approaches, morphing weights, source databases, and image quality. The testing protocols of the database are listed below.

| Protocols | Training                          |  Testing                              |
| :--:      | :--:                              | :--:                                  |
| 1         | the images of one morphing type   | the images of the same morphing type  |
| 2         | the images of one morphing type   | the images of unseen morphing types   |
| 3         | the images from ND-IIITD database | the images from self-collected images |
| 4         | high-resolution probe images      | low-resolution probe images           |
| 5         | frontal probe face images         | non-frontal probe face images         |

## How to get access to the database?

If you are interested in the database, please read the [database release agreement](https://github.com/pp21/feaws_mad/blob/main/agreement.pdf) and send your request to the corresponding author of the database. Thank you.

## References

[1] Makrushin A, Neubert T, Dittmann J. Automatic Generation and Detection of Visually Faultless Facial Morphs. International Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications (VISIGRAPP), 2017: 39-50.

[2] Ferrara M, Franco A, Maltoni D. Face demorphing. IEEE Transactions on Information Forensics and Security, 2018, 13(4): 1008-1017.

[3]	Neubert T, Makrushin A, Hildebrandt M, et al. Extended stirtrace benchmarking of biometric and forensic qualities of morphed face images. IET Biometrics, 2018, 7(4): 325-332.
