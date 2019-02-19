# Nobile-Hernday Bioinformatics Workshop [Feb 19, 2019]
<br />

![alt text](https://raw.githubusercontent.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/master/Relevant-Articles_Figures-of-Interest-Highlighted/Nobile-Lab_UC-Merced.png) 
This is an introduction tutorial on bioinformatics, tailored to Nobile and Hernday lab members. <br />
Contributors: Sabah Ul-Hasan ([@sabahzero](https://github.com/sabahzero)) and Akshay Paropkari ([@akshayparopkari](https://github.com/akshayparopkari))

## Overview and aims of today
09:00 - 09:30 AM Introduction, validation of Jupyter and Git installation of personal computer </br>
09:30 - 10:30 AM Basics, creating a growth curve and heatmap, changing color schemes, etc </br>
10:30 - 11:00 AM Integration and connection to the MERCED cluster, general Q&A (joined by Matthias Bussonnier) </br>

### 9 - 9:30 AM Introduction, validation of Jupyter and Git installation of personal computer
Background: What are Jupyter and Git, and why use them? What do they have to do with <i>C. abicans</i>, for example? </br> </br>
  Jupyter is essentially a lab notebook for 'big data' (ie sequencing -omics). We can think of it as the 'Box' or 'Dropbox' of coding and bioinformatics. The sooner and better we are with keeping good bioinformatics notes, the sooner and better we can be with reproducible research, improving and building off of findings from any given project - much like you would do with a wetlab experiment. Read more about Jupyter and its uses from this recent [Nature article](https://www.nature.com/articles/d41586-018-07196-1). </br> </br> 
  We all understand how to create a "New Folder" on our desktop. Command line essentially acts as the 'blueprint' or code behind how those New Folders come into existence. We see them as an icon right away, and a few lines of code are what make them appear in a user-friendly way. This is known as [version control](https://www.atlassian.com/git/tutorials/what-is-version-control). Git takes version control a step further. Git makes version control easy to collaborate and share, such as with other scientists. Again, this also helps with making one's work more reproducible and accessible (just like with Box or Dropbox!). Learn more about Git [here](https://git-scm.com/video/what-is-git). </br> </br> 
  Today we will be installing both Jupyter notebook and Git onto our personal computers to help use work with and share our data more easily. Don't worry if all this seems extremely confusing at the moment. The reasoning will become clearer throughout the tutorial, but also don't hesitate to ask questions at any time. There are multiple people in the room who are very happy to help and explain in whatever way suits you best! On that note, if you see something in tutorial that could easily be improved then feel free to create a [Pull Request](https://help.github.com/articles/creating-a-pull-request/) at any time and we will incorporate it -- the benefit of open-source and Git already demonstrated in real-time!<br>
  1. Confirm access to a command line prompt for your computer </br>
  If you're not sure how to use or access this, check out this [quick introduction](https://www.davidbaumgold.com/tutorials/command-line/)</br> 
  Let's do a "fun" test by seeing if we can find our Desktop folder through command line </br> </br>
  Checkpoint A </br> 
  
  2. Install Jupyter </br>
  Jupyter requires Python and Anaconda before it can be installed successfully. This may seem like extra work now, but many bioinformatics data and progams involve Python and/or Anaconda. So, in the long-term, you'll already be prepared! </br>
  Install [Python](https://www.python.org/downloads/) This is a programming language, analogous to R. We will be using R in the tutorial because it's a language more commonly used in the life science, but python is certainly the way to go if you're considering being more involved in bioinformatics and/or the tech industry in the long-term. This is because most in those "realms" use Python. The whole reason we need to install Python is because Jupyter notebook was written in Python! </br>
  Install [Anaconda](https://www.anaconda.com/distribution/) This is a platform that will help your usage of Python or R, and associated packages, run faster and smoother. Now for the big reveal: Install [Jupyter Notebook](https://jupyter.org/install) </br>
  Alright, are you ready for this? After typing-in </br>`jupyter notebook`</br> in command line, do you see your Desktop folder in the pop-up browser? Pretty cool, huh?! *note* this does mean you have to be connected to the internet when using the notebook, but you'll see why this is can be a great alternative to software such as RStudio shortly. </br> </br>
  Checkpoint B </br> 
  
  3. Ensure R is part of your Jupyter notebook (not just Python) </br>
  Let's create a new R notebook. Oops! We only see Python. </br>
  Fear not, here's [a tutorial](https://www.datacamp.com/community/blog/jupyter-notebook-r) on how to install R as part of your notebook. You can also copy/paste the below into a new command-line prompt, which is the same as the section option in the tutorial). Be sure to close your notebook, just in case. </br>
  `conda install -c r r-essentials`</br> 
  Re-open your notebook. You should now see an option to create an R notebook: 
  ![alt text](https://raw.githubusercontent.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/master/Relevant-Articles_Figures-of-Interest-Highlighted/Jupyter-Notebook_R-console.png) 
  We're not going to make an R Jupyter notebook (because one has already been made for you here, yay!). We are going to download this, and all files in the tutorial repository using Git</br> </br>
  Checkpoint C </br> </br> 
  
  4. Install Git </br>
  Okay, things are about to get interesting. See the .ipynb file in this repository (scroll the the tippy-top)? That's the file containing everything we need for the notebook. We're going to download it, and everything in this tutorial repository (which contain the reference data and figures), and move it into Desktop with just a few quick command lines. But first! We need Git to do it. </br>
  [Installation instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) </br>
  Open a new command line prompt, type </br>
  `ls`</br> 
  We want to be in our Desktop. To get there, type </br>
  `cd Desktop/`</br> 
  Type `ls` again, to double-check it aligns with what you see on your home screen </br>
  Congratulations on what may be your first version control experience! </br>
  Now type `git init` to initiate Git in your Desktop </br> 
  Visit the repository site and click on the drop-down arrow in the "Clone or download" green button </br>
  *note* make sure you 'Clone with HTTPS' (easy to back-track this way over SSH if you make a mistake in your own repo) </br>
  ![alt text](https://raw.githubusercontent.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/master/Relevant-Articles_Figures-of-Interest-Highlighted/Download-Folder_Git.png) 
  Now type (in your terminal on your computer) </br>
 `git clone https://github.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019.git` </br>
 *note* the https link above should match the same linke from the drop-down arrow. </br> 
 We are copying and downloading it, using Git! </br>
 This will take a few minutes. </br>
 Open up your Desktop folder as you usually would on your computer. *cue drum-roll* </br>
 Do you see a Folder labeled "Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019" ? </br> 
 This should also show up in your Jupyter notebook. </br> </br>
  Checkpoint D </br> </br> 
 
 5. Open your .ipynb (Jupyter notebook set-up in R language) in your Jupyter notebook browser </br>
 Is this what you see in the first section? Try it out, give it a run! </br>
 ![alt text](https://raw.githubusercontent.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/master/Relevant-Articles_Figures-of-Interest-Highlighted/Jupyter-Notebook-R.png) 
 Congratulations, you just ran a piece of R code!!! 😃 </br></br> 
  Checkpoint E </br> </br> 
 
Why do all this? </br>
- You don't need to know any code to create the figures we're about to make in the notebook, and it's *much* faster than using Excel. </br>
- You can easily adjust the code in your notebook for colors, axes, etc and see it quickly without having to use RStudio or run the entire code in R </br>
- You can easily share your workflow with anyone else who uses Jupyter notebook, just as I've done here. This improves reproducibility, and can dramatically reduce many hours spent on trouble-shooting (especially in a big group, such as the Nobile and Hernday labs!) </br>
- The [MERCED cluster](http://hpcwiki.ucmerced.edu/knowledgebase/merced-cluster-user-manual/) will soon be integrating [Jupyter Hub](https://www.google.com/search?client=firefox-b-1-d&q=jupyter+hub). It's not yet available, which is why we're using our personal computers today, but when it is you will be able to use a notebook simply by browser log-in (much like Box or DropBox) from *any* computer anywhere! Akshay will go more into using the cluster at the end of the workshop, and [Matthias Bussonnier](http://hpcwiki.ucmerced.edu/knowledgebase/hpc-walk-in-clinics/) will also be sitting in for any questions we may have</br> </br>
More info on R, in case you're interested [here](https://www.rstudio.com/resources/cheatsheets/) for code cheatsheets and [here](https://www.r-graph-gallery.com/) for coding visuals

### 9:30 - 10:30 AM Basics, creating a growth curve and heatmap, changing color schemes
6. This will involve [our Jupyter notebook](https://github.com/sabahzero/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019/blob/master/Nobile-HerndayLabs_BioinformaticsWorkshop_Feb19-2019.ipynb) for the rest of the time. Ideally, at this stage you are able to run this through your own personal computer such that you will be able to adjust and edit accordingly. If not, no worries! Click on the previous hyper-link and you can follow along that way, too. No need to be sitting around feeling bored! </br> </br> 

We will focus on growth curve graphs from culture data and heatmaps from RNA-Seq data, but feel free to play with the sections on histograms, bar charts, boxplots, and/or venn-diagrams if you already know how to do these! </br>  </br> 

Checkpoint F </br> </br> 

RNA-Seq analysis in R [resource](http://combine-australia.github.io/RNAseq-R/)</br> 
CHIP-Seq analysis in R [resource](https://link.springer.com/protocol </br> 


### 10:30 - 11:00 AM Integration and connection to the MERCED cluster ([manual](http://hpcwiki.ucmerced.edu/knowledgebase/merced-cluster-user-manual/)), general Q&A
7. To access the MERCED cluster, open your command line prompt</br>
&nbsp;&nbsp;&nbsp;a. For Linux/MacOS - open Terminal app</br>
&nbsp;&nbsp;&nbsp;b. For Windows - install [Git for Windows](https://gitforwindows.org/) </br>
ssh `your_username`@merced.ucmerced.edu</br>
Enter your MERCED password, when prompted </br> </br>
[UNIX basics](https://swcarpentry.github.io/shell-novice/)</br> </br>
Transfer files between the local machine (your laptop/desktop) to MERCED</br>
&nbsp;&nbsp;&nbsp;a. scp `source_fullpath` `destination_fullpath` (PREFERRED method)</br>
&nbsp;&nbsp;&nbsp;b. sftp `source_fullpath` `destination_fullpath` [more information](http://hpcwiki.ucmerced.edu/knowledgebase/how-to-transfer-files-to-or-from-the-cluster/)</br> </br>

Checkpoint G </br></br>

Getting started with Open Reproducible Science [(OCR)](https://www.earthdatascience.org/courses/earth-analytics-bootcamp/get-started-with-open-science/jupyter-notebook-interface/)</br>
Introduction to [Shell](https://hbctraining.github.io/Intro-to-Shell/schedule/) </br>

### Contacts
Sabah Ul-Hasan ([@sabazhero](https://github.com/sabahzero)) </br>
Akshay Paropkari ([@akshayparopkari](https://github.com/akshayparopkari)) </br>
Thaddeus Seher ([@tdseher](https://github.com/tdseher))</br>
Matthias Bussonnier ([@Carreau](https://github.com/Carreau))</br>
[Sarvani Chadalapaka](https://it.ucmerced.edu/content/sarvani-chadalapaka) 
