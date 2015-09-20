A few implementations of kernel methods,  datasets, and publications.

**All the codes here are provided "AS IS", without any guarantee. Do not try to sue me!**

**Datasets**:
  * MNIST Handwritten Digits http://kernelmachine.googlecode.com/files/mnist_all.mat (from Sam Roweis' webpage)
> > 8-bit grayscale images of "0" through "9"; about 6K training examples of each class; 1K test examples
  * USPS Handwritten Digits http://kernelmachine.googlecode.com/files/usps_all.mat (from Sam Roweis' webpage)
> > 8-bit grayscale images of "0" through "9"; 1100 examples of each class.
  * Binary Alphadigits http://kernelmachine.googlecode.com/files/binaryalphadigs.mat (from Sam Roweis' webpage)
> > Binary 20x16 digits of "0" through "9" and capital "A" through "Z". 39 examples of each class.From Simon Lucas', Algoval system.
  * 20 Newsgroups http://kernelmachine.googlecode.com/files/20news_w100.mat (from Sam Roweis' webpage)
> > A tiny version of the 20newsgroups data, with binary occurance data for 100 words across 16242 postings. Sam Roweis has also tagged the postings by the highest level domain in the array "newsgroups".
The credits go to Sam Roweis for the above datasets.
    * The classification data http://kernelmachine.googlecode.com/files/classification_data.txt contains 200 data, sampled from a 3-component Gaussian mixture in 2D. This data was generated using the gmmsamp function from Netlab. The corresponding Gaussian mixture model had the parameters:
```
mix.priors = [0.5 0.25 0.25];
mix.centres = [0 -0.1; 1 1; 1 -1];
mix.covars(:,:,1) = [0.625 -0.2165; -0.2165 0.875];
mix.covars(:,:,2) = [0.2241 -0.1368; -0.1368 0.9759];
mix.covars(:,:,3) = [0.2375 0.1516; 0.1516 0.4125];
```
The first component represent class 1 (blue circles, o, in the left panel of Figure A.7), the other components class 0 (red crosses, ×). The file has 200 rows of 3 columns, the first two columns giving datum position, the last column containing the label (0/1).
    * Training data for robust face detection using boosting http://kernelmachine.googlecode.com/files/viola-traindata.tar.gz, as formalized by Viola and Jones. Includes Matlab code for reading the data. Credits go to Viola, Jones and Peter Carbonetto.
    * Sparse coded images from Caltech256 http://kernelmachine.googlecode.com/files/Caltech256.tar.gz Images are represented using "visterms", a combination of color and texture histograms.