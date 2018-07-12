# Research Project

## Synopsis

The goal of this project is to replicate the results of a previously published computational photography paper. Replication provides a deeper understanding of research results, and allows you to compare your results against an expected baseline. While previous results are helpful as a guide towards implementation, successful replication can be challenging. Instructions are not always clear, and implementation details like parameter values may be missing or ambiguous, and it is sometimes difficult or impossible to achieve exactly the same results.


## Instructions

Your assignment is to replicate the published results of [Seam Carving for Content-Aware Image Resizing](http://www.faculty.idc.ac.il/arik/SCWeb/imret/index.html) by Shai Avidan and Ariel Shamir. (There is a PDF copy of the paper in the course resources on Piazza.) You will deliver:

  - **Your own** implementation of the seam carving algorithm

  - A 2-3 page (3 page max) written report

  - A short (3 minutes max) video presentation

Your report and presentation should include a brief description of the experiment, an overview of your implementation, and presentation of your results in comparison to those in the original paper (including any significant differences). Be sure to describe any issues you encountered while trying to replicate the results (e.g. ambiguous instructions, results that differ wildly from the published results) and explain how you overcame them. You must show:

  - Seam removal (Figure 5 -- you do *not* need to show scaling or cropping)

  - Implement optimal retargeting with dynamic programming (Figure 7 -- show the transport map with your seam removal path & the result of optimal retargeting; you are not required to show the other three versions using alternating row/col seam removal)

  - Seam insertion (Figure 8 -- parts c, d, and f only)


**NOTES:**

- **Details on the code:**
  - You may use any language of your choice as long as it compiles and runs on the course VM, and you may use 3rd party libraries for image file I/O and linear algebra as required.
  - Your submission must include all source code, support libraries, and *complete* instructions included in a README file to execute your code on the course VM. ("Complete" means that every required step must be explicit in your instructions; e.g., do NOT say "install `customImageLibrary`", instead give the **exact** command -- we should be able to copy/paste your instructions to get setup.)

- **Details for the report:**
  - The report must be in PDF format; no other format will be accepted.
  - There is no required template for the report; however, the format should be approximately equivalent to something like aaai or nips format (see the [templates](/Research_Project/templates) folder for reference).  *You are NOT required to use TeX; the templates are provided for reference.*
  - If you do not use one of the provided templates, font size should be at least 10pt and margins at least 1"; single-spaced, single column.
  - You do not need a title page, cover page, etc.
  - Include a link to your video.

- **Details for the video:**
  - The video must be uploaded to an internet hosting platform.
  - Make sure that the link is not searchable, and that it is shared properly (i.e., only you and people with the link should be able to access it).
  - Do not speed up your presentations to compress the time.

- We are serious about the 3 pages and 3 minutes limit. A report of 3 pages and one line will cost you points. A video of length 3:01 will cost you points.


## Submit the Project

Save your report in the project direcotry as `report.pdf`, and put your source code and supporting files in a file named `resources.zip` -- both files are required.  If your code has library dependencies or setup instructions that are required to run it on the VM, then your resources file **must** include instructions in a plaintext file named "README.txt". (These names are important because the submission script searches the current working directory for exact matches to the filenames). You will not submit your video file; it must be hosted on youtube, google drive, dropbox, or similar. 

**ATTENTION:** Make sure you include a link to your video clearly in your report. Also make sure you have permissions set to allow TAs to access your video or there will be a substantial deduction.

**Note:** Make sure that you have completed all the steps in the [instructions](../README.md#virtual-machine-setup) for installing the VM & other course tools first.

Follow the [Project Submission Instructions](../README.md#submitting-projects) to upload your report from the course VM to [Bonnie](https://bonnie.udacity.com) using the `omscs` CLI.

  - Submit your report with the CLI on the VM from within the project folder:

```
$ omscs submit report
```

**Note:** The total size of your project (report + resources) must be less than 30MB for this project. If your submission is too large, you can reduce the scale of your images or report.


## Evaluation Criteria

Your work will be graded on:
  - Your understanding of the original paper
  - The quality of your replication results
  - The quality of your report & presentation
