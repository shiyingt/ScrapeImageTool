# ScrapeImageTool
Download Images from Search Engine - intended use for datasets to train ML models

I needed image datasets to train Machine Learning Models but ImageNet was down. So I created a tool to   
(1) get me links of images  
(2) download the images from the link onto my computer  

I did   
(1) using python on juypter notebook, beautiful soup and selenium  
(2) bash script  

## user guide 
the jupyter notebook takes the input of the search engine website and returns the concatenated form of the image links.  
replace the first line of the bash script with the concatenated form of the image links.  
in your linux terminal, enable the execute permission on the bash file. if you use windows, check how to enable linux subsystems on windows.  
`chmod +x filename.sh`  
then, run the bash script. the images would appear in the same file that you run your bash script in.  
`./filename.sh`  
remember to do a quick check through on the images you have downloaded before you use the images to train the models as some images may not be accurate to the search term!

## other notes
I chose to rename the images i downloaded when using wget was because some of the images that i downloaded had names with weird characters which did not allow me to zip the file - which has a big size as it contained images.  
if you want enabled linux subsystems on windows and would like to get to your local C drive, you can do so with  
`cd /mnt/c`  
another note to self is to check hackathon details before committing because i only realised that i wasn't able to join the hackathon after preparation done for the demo :(
