Problem 4

a) The JPEG image contains different quantization levels for q=1,2,3,4 and 8.
   The corresponding .pgm files are also in the same folder. 
   With higher quantization-levels the quality of the image gets better.
b) We integrated the code into the corresponding locations...
c) In the folders "4c1results" and "4c2results" there's also a JPEG image of
   the differently filtered images. The MSE and PSNR values are provided in the 
   .txt files. 
   We can observe, that with rising quantization levels the impact of noise gets
   diminished. The higher the quality of a particular image the smaller the 
   MSE and the higher the PSNR value become. 
   Note: The PSNR values are logarithmic so the proportion of the values aren't linear.

Problem 5

a) The original striped image wraps around if you surround it by copies of itself.
   So there aren't any sharp edges that would result in artefacts or lines in the FFT image.
   We can observe here that the fourier transformed image has dots of the according frequencies
   in such an orientation that matches the direction of the stripes. It appears that the top and bottom 
   arrangements of the dots correspond to the FFT in y-direction and the middle array to the x-direction.
b) As the gauss3.pgm doesn't wrap around itself (smoothly) there are sharp edges wich are interpreted
   by the FFT as high frequency parts and so they get plotted as vertical and horizontal lines
   (x and y directions). This effect could be canceled by applying a "vignette" effect to that image.
c) The aliasing artifacts are clearly visible as lines that go inside the image starting right at the edges.
   They look like parts of a neighbor DFT that creep over inside that image.
   (We've highlighted some of them with red color in the artifacts.jpg image)