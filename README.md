# Nobile-Hernday Bioinformatics Workshop [Feb 19, 2019]
<br />

![alt text](https://raw.githubusercontent.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/master/Relevant-Articles_Figures-of-Interest-Highlighted/Nobile-Lab_UC-Merced.png) 
This is an introduction tutorial on bioinformatics, tailored to Nobile and Hernday lab members. <br />
Contributors: Sabah Ul-Hasan ([@sabahzero](https://github.com/sabahzero)) and Akshay Paropkari ([@akshayparopkari](https://github.com/akshayparopkari))

## Overview and aims of today
09:00 - 09:30 AM Introduction, validation of Jupyter and Git installation of personal computer </br>
09:30 - 10:30 AM Basics, creating a growth curve and heatmap, changing color schemes, etc </br>
10:30 - 11:00 AM Integration and connection to the MERCED cluster, general Q&A </br>

### 9 - 9:30 AM Introduction, validation of Jupyter and Git installation of personal computer
Background: What are Jupyter and Git, and why use them? What do they have to do with <i>C. abicans</i>, for example? </br> </br>
  Jupyter is essentially a lab notebook for 'big data' (ie sequencing -omics). We can think of it as the 'Box' or 'Dropbox' of coding and bioinformatics. The sooner and better we are with keeping good bioinformatics notes, the sooner and better we can be with reproducible research, improving and building off of findings from any given project - much like you would do with a wetlab experiment. Read more about Jupyter and its uses from this recent [Nature article](https://www.nature.com/articles/d41586-018-07196-1). </br> </br> 
  We all understand how to create a "New Folder" on our desktop. Command line essentially acts as the 'blueprint' or code behind how those New Folders come into existence. We see them as an icon right away, and a few lines of code are what make them appear in a user-friendly way. This is known as [version control](https://www.atlassian.com/git/tutorials/what-is-version-control). Git takes version control a step further. Git makes version control easy to collaborate and share, such as with other scientists. Again, this also helps with making one's work more reproducible and accessible (just like with Box or Dropbox!). Learn more about Git [here](https://git-scm.com/video/what-is-git). </br> </br> 
  Today we will be installing both Jupyter notebook and Git onto our personal computers to help use work with and share our data more easily. Don't worry if all this seems extremely confusing at the moment. The reasoning will become clearer throughout the tutorial, but also don't hesitate to ask questions at any time. There are multiple people in the room who are very happy to help and explain in whatever way suits you best! On that note, if you see something in tutorial that could easily be improved then feel free to create a [Pull Request](https://help.github.com/articles/creating-a-pull-request/) at any time and we will incorporate it -- the benefit of open-source and Git already demonstrated in real-time!<br>
  1. Confirm access to a command line prompt for your computer </br>
  If you're not sure how to use or access this, check out this [quick introduction](https://www.davidbaumgold.com/tutorials/command-line/)</br> 
  Let's do a "fun" test by seeing if we can find our Downloads folder through command line </br> </br>
  Checkpoint A </br> 
  
  2. Install Jupyter </br>
  Jupyter requires Python and Anaconda before it can be installed successfully. This may seem like extra work now, but many bioinformatics data and progams involve Python and/or Anaconda. So, in the long-term, you'll already be prepared! </br>
  Install [Python](https://www.python.org/downloads/) This is a programming language, analogous to R. We will be using R in the tutorial because it's a language more commonly used in the life science, but python is certainly the way to go if you're considering being more involved in bioinformatics and/or the tech industry in the long-term. This is because most in those "realms" use Python. The whole reason we need to install Python is because Jupyter notebook was written in Python! </br>
  Install [Anaconda](https://www.anaconda.com/distribution/) This is a platform that will help your usage of Python or R, and associated packages, run faster and smoother. Now for the big reveal: Install [Jupyter Notebook](https://jupyter.org/install) </br>
  Alright, are you ready for this? After typing-in </br>`jupyter notebook`</br> in command line, do you see your Downloads folder in the pop-up browser? Pretty cool, huh?! *note* this does mean you have to be connected to the internet when using the notebook, but you'll see why this is can be a really great alternative to software such as RStudio shortly </br> </br>
  Checkpoint B </br> 
  
  2. Ensure R is part of your Jupyter notebook (not just Python)
  3. Install Git
  4. Use Git to download and move the .ipynb file from this tutorial repository to your personal computer
 
1. Exposure to R, GitHub, and Jupyter as complementary tools for data analysis over using Excel </br>
&nbsp;&nbsp;&nbsp;a. What is R, and why use it as a scientist? Read introduction article [here](https://www.r-project.org/about.html) </br> 
&nbsp;&nbsp;&nbsp;b. The power of Git and Github as an open-source interface used with R: [Nature article](http://blogs.nature.com/naturejobs/2018/06/11/git-the-reproducibility-tool-scientists-love-to-hate/) </br> 
&nbsp;&nbsp;&nbsp;c. Using Jupyter notebook as a reproducible bioinformatics 'lab notebook': [Nature article](https://www.nature.com/articles/d41586-018-07196-1) </br>

### Basics, creating bar plots with standard error, changing color schemes, etc
2. Using Jupyter notebook to run R code for RNA-Seq data analysis, and interacting with Gihtub as an interface </br> 
&nbsp;&nbsp;&nbsp;a. RNA-Seq analysis in R [resource](http://combine-australia.github.io/RNAseq-R/)</br> 
&nbsp;&nbsp;&nbsp;b. CHIP-Seq analysis in R [resource](https://link.springer.com/protocol/10.1007%2F978-1-4939-7380-4_17)</br> 
3. Using Jupyter notebook and R code to create publish-ready figures from an Excel datasheet for: </br>
&nbsp;&nbsp;&nbsp;a. Growth curves and scatter plots </br>
&nbsp;&nbsp;&nbsp;b. Bar charts, boxplots, and histograms with significance vs variance </br>
&nbsp;&nbsp;&nbsp;c. Heatmaps with significance vs variance </br>
&nbsp;&nbsp;&nbsp;d. Co-occurrence, network graphs, and venn diagrams with significance vs variance </br>

We will primarily be working with RNA-Seq Data </br>
Follow along by clicking on the file labeled "Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019.ipynb" or [link here](https://github.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/blob/master/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019.ipynb)

### Overview of the MERCED cluster, how to use it through command line, why and general Q&A
4. Running shell</br>
&nbsp;&nbsp;&nbsp;a. For Linux/MacOS - open Terminal app</br>
&nbsp;&nbsp;&nbsp;b. For Windows - install [Git for Windows](https://gitforwindows.org/)

5. ACCESSING MERCED</br>
&nbsp;&nbsp;&nbsp;a. ssh `your_username`@merced.ucmerced.edu</br>
&nbsp;&nbsp;&nbsp;b. Enter your MERCED password, when prompted

6. [UNIX basics](https://swcarpentry.github.io/shell-novice/)</br>

7. Transferring files between local machine (your laptop/desktop) to MERCED</br>
&nbsp;&nbsp;&nbsp;a. scp `source_fullpath` `destination_fullpath` (PREFERRED method)</br>
&nbsp;&nbsp;&nbsp;b. sftp `source_fullpath` `destination_fullpath` [more information](http://hpcwiki.ucmerced.edu/knowledgebase/how-to-transfer-files-to-or-from-the-cluster/)</br> 

8. [MERCED user manual](http://hpcwiki.ucmerced.edu/knowledgebase/merced-cluster-user-manual/)

### Miscellaneous resources
- Getting started with Open Reproducible Science [(OCR)](https://www.earthdatascience.org/courses/earth-analytics-bootcamp/get-started-with-open-science/jupyter-notebook-interface/)
- [Introduction to Shell](https://hbctraining.github.io/Intro-to-Shell/schedule/)
