# Familiarity Rating Experiment
This is a simple project that uses jsPsych to collect familiarity ratings for a set of images.

The main experiment is housed in the "index.html" file. This file defines and runs the experiment. 
This experiment needs:
* the necessary jsPsych libraries (jsPsych-6.1.0/)
* the necessary jQuery file (jquery-3.5.1.js -- used for certain functionality)
* the "write_data.php" file (saves the data)
* the images used in the experiment (housed in folder called "ganfaces_final/" -- ask Ivette for access to this image folder) 

The "index.html" file is easily editable for your own use-- swap out stimuli files, edit survey questions, etc.-- However, I recommend building an experiment from scratch using jsPsych if you can.
It's remarkably simple and customizable, although it may take a bit of Googling and a couple of hours to get the hang of it. It's worth it, though! This very experiment started from a simple tutorial: https://www.jspsych.org/tutorials/hello-world/.
You can download the necessary jsPsych libraries (6.1.0) for this experiment from their website.


### To run this experiment on a server (like Sapir):
1. Login to the server on the UW Madison VPN using your credentials (ask Dr. Ward for your login)
2. Navigate to the mturk experiments directory ("cd /var/www/mturk")
3. Make a new folder in this directory ("mkdir new_folder_name") // call it whatever you want ~
4. Inside /var/www/mturk/new_folder_name, make a folder called "html" ("mkdir html")
5. Inside of /var/www/mturk/new_folder_name/html, make a folder called "data", give this folder write access ("chmod gou+wrx data/")
4. Collect all of the files and directories above (index.html, jsPsych libraries, jquery-3.5.1.js, write_data.php, ganfaces_final folder with all images), and put them into a central folder called "html" on your computer
5. Copy the html folder on your computer into the new_folder_name/html directory on the server (use the "scp" function from your computer to the server)
6. Navigate to the webpage! (something like sapir.psych.wisc.edu/mturk/new_folder_name/html)
