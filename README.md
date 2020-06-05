# PSNR-Peak-Signal-to-Noise-ratio-CALCULATION
The term peak signal-to-noise ratio (PSNR) is an expression for the ratio between the maximum possible value (power) of a signal and the power of distorting noise that affects the quality of its representation.

PSNR is most easily defined via the mean squared error (MSE). Given a noise-free m×n monochrome image I and its noisy approximation K, MSE is defined as:

{\displaystyle {\mathit {MSE}}={\frac {1}{m\,n}}\sum _{i=0}^{m-1}\sum _{j=0}^{n-1}[I(i,j)-K(i,j)]^{2}}{\mathit  {MSE}}={\frac  {1}{m\,n}}\sum _{{i=0}}^{{m-1}}\sum _{{j=0}}^{{n-1}}[I(i,j)-K(i,j)]^{2}
The PSNR (in dB) is defined as:

{\displaystyle {\begin{aligned}{\mathit {PSNR}}&=10\cdot \log _{10}\left({\frac {{\mathit {MAX}}_{I}^{2}}{\mathit {MSE}}}\right)\\&=20\cdot \log _{10}\left({\frac {{\mathit {MAX}}_{I}}{\sqrt {\mathit {MSE}}}}\right)\\&=20\cdot \log _{10}\left({{\mathit {MAX}}_{I}}\right)-10\cdot \log _{10}\left({\mathit {MSE}}\right)\end{aligned}}}{\begin{aligned}{\mathit  {PSNR}}&=10\cdot \log _{{10}}\left({\frac  {{\mathit  {MAX}}_{I}^{2}}{{\mathit  {MSE}}}}\right)\\&=20\cdot \log _{{10}}\left({\frac  {{\mathit  {MAX}}_{I}}{{\sqrt  {{\mathit  {MSE}}}}}}\right)\\&=20\cdot \log _{{10}}\left({{\mathit  {MAX}}_{I}}\right)-10\cdot \log _{{10}}\left({{{\mathit  {MSE}}}}\right)\end{aligned}}
Here, MAXI is the maximum possible pixel value of the image. When the pixels are represented using 8 bits per sample, this is 255. More generally, when samples are represented using linear PCM with B bits per sample, MAXI is 2B−1

For color images with three RGB values per pixel, the definition of PSNR is the same except the MSE is the sum over all squared value differences (now for each color, i.e. three times as many differences as in a monochrome image) divided by image size and by three. Alternately, for color images the image is converted to a different color space and PSNR is reported against each channel of that color space, e.g., YCbCr or HSL.
