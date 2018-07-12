#Image Resizing
Goal: Increase/decrease the size of the image

#Process:
1. Determine size change of image (width or height) and by how many rows/columns
2. If increasing/decreasing height..rotate image
3. Create energy map of image
4. Determine vertical seams that have the minimum cumulative energy based on size change
5. If decreasing, remove seams from image and repeat steps 1-4
6. If increasing size, put seams in array, repeat steps 1-5, then add all minimum energy seams to original image

#To run:
1. From root directory run the command:
	 python start.py
2. Provide the name to the image you want to alter that MUST be in the src folder
3. Provide the dimensions you want to change the image to
4. All output files will be placed into the output directory

#Before runnig you must install the following libraries:
pip install imutils 
