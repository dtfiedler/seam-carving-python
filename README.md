# Research Project

## Synopsis

The goal of this project is to replicate the results of a previously published computational photography paper. Replication provides a deeper understanding of research results, and allows you to compare your results against an expected baseline. While previous results are helpful as a guide towards implementation, successful replication can be challenging. Instructions are not always clear, and implementation details like parameter values may be missing or ambiguous, and it is sometimes difficult or impossible to achieve exactly the same results.


## Assignment Instructions

Your assignment is to replicate the published results of [Seam Carving for Content-Aware Image Resizing](http://www.faculty.idc.ac.il/arik/SCWeb/imret/index.html) by Shai Avidan and Ariel Shamir. (There is a PDF copy of the paper in the course resources on Piazza.) You will deliver:

  - **Your own** implementation of the seam carving algorithm

  - A 2-3 page (3 page max) written report

  - A short (3 minutes max) video presentation

Your report and presentation should include a brief description of the experiment, an overview of your implementation, and presentation of your results in comparison to those in the original paper (including any significant differences). Be sure to describe any issues you encountered while trying to replicate the results (e.g. ambiguous instructions, results that differ wildly from the published results) and explain how you overcame them. You must show:

  - Seam removal (Figure 5 -- you do *not* need to show scaling or cropping)

  - Implement optimal retargeting with dynamic programming (Figure 7 -- show the transport map with your seam removal path & the result of optimal retargeting; you are not required to show the other three versions using alternating row/col seam removal)

  - Seam insertion (Figure 8 -- parts c, d, and f only)

## Results

### Seam Removal:
#### Original Image
![orig_image](https://github.com/dtfiedler/seam-carving-python/blob/master/resources/beach_orig.png)

#### Seams Removed
![orig_image](https://github.com/dtfiedler/seam-carving-python/blob/master/resources/beach_350_final.png)

### Seam Insertion
~[orig_image](https://github.com/dtfiedler/seam-carving-python/blob/master/resources/fig8.png)

![seams](https://github.com/dtfiedler/seam-carving-python/blob/master/resources/seam_overlay.png)

![result](https://github.com/dtfiedler/seam-carving-python/blob/master/resources/expanded_478_final_output.png)

## Process:
1. Determine size change of image (width or height) and by how many rows/columns
2. If increasing/decreasing height..rotate image
3. Create energy map of image
4. Determine vertical seams that have the minimum cumulative energy based on size change
5. If decreasing, remove seams from image and repeat steps 1-4
6. If increasing size, put seams in array, repeat steps 1-5, then add all minimum energy seams to original image

## To run:
1. From root directory run the command:
	 python start.py
2. Provide the name to the image you want to alter that MUST be in the src folder
3. Provide the dimensions you want to change the image to
4. All output files will be placed into the output directory

NOTE: Before runnig you must install the following libraries:
pip install imutils 
