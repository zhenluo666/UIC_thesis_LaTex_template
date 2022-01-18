# LaTex Template for Thesis at UIC
## Intro
This LaTex template is served as a useful starting point for writing a PhD thesis at University of Illinois at Chicago (UIC). Its structure and format has been modified and updated to abide by the requirement of thesis manual released by Graduate College since 2016.  
The templated (Document class) was initially developed by Paul Davis at 1991, followed by a series of updates from Ethan Munson, Thomas McKibben, Nathan Bliss, Pete Snyder and Zhen Luo.  
A LaTex editor (w/ GUI) is strongly suggested for editing and typesetting, such as TexPad, along with standard LaTex packages for building. 

### Repo structure
The format and layout of template are well established so you should only need to edit a few files. However, here I will still give a full list of files in folder with respective descriptions:
#### 1. ThesisManual_rev_06Oct2016.pdf
This is the latest thesis manual in 2021 released by Graduate College, with all required format details and samples included. Please refer to the latest version if there is further release.
#### 2. forma.bst, formb.bst, formc.bst
These are available bibliography styles for reference. No need to make any changes to these files. You will be able to choose one of them when setting the reference style at section {Begin Document} in thesis.tex. Please refer to the comment description in corresponding position.
#### 3. uicth11.clo, fontsym.tex
These are font style related files. No need to make any changes.
#### 4. uicthesi.cls
This is document class file that defines the structure of thesis with specific format encoded. Generally, no need to make any changes. However, do comply with latest format requirement and make changes if needed. In such case, use search to locate the lines and keep the original code commented while updating the new format. Proper documentation of code is the key.
#### 5. README.md (within the folder)
This is a README file developed by Pete Snyder, with description of some files. This is the reason why I'm presenting current README with comprehensive description of all files.
#### 6. Makefile
This is used for compiling LaTex files into PDF. No need to touch it.
#### 7. /figures
This is the folder that stores all the figures you will be using in the thsis. In the thsis.tex, just map to the directory/address of these figures as example shows and the template will create the figure structure and figure table for you automatically. In addition, I would suggest to create sub-folders in /figures to separate different chapters.
#### 8. /sections
This is the folder that stores all the chapters and other sections of thesis. If you are using a GUI like TexPad, then no need to touch this folder because you are able to edit them in GUI. This folder will show you the mapping of different sections in thesis. If not using a GUI, then edit your chapters or add more chapters in this section folder.
##### --- main chapters
In the template, I already create two chapters (introduction and sample chapter) for you. Add more chapters by making copy of them. Please note for each chapter, there should have a 0_index.tex as a index file that defines the structure of all sub-chapters within current chapter. Also, it defines the name and lable (in case you want to mention this chapter somewhere else, then just call \label) of current chapter.
##### --- other
This sub-folder includes all other minor sections in the thsis, such as dedication, acknowlegement, summary, vita, etc. Please refer to the comments within each file (with index 1-5).  
`__preamble.tex` is the file where you want to insert any other LaTex packages  
`__commands.tex` is the file where you want to create new commands  
`__abbrs.tex` is the file where you want to create abbreviations in thesis. This is useful and please refer to the examples within the file  
#### 9. thesis.bib
This is collection of all your reference in the format of bib. Call the label of each reference in thesis.tex and it will create the reference table and labels for you automatically. Please refer to the examples in thesis.tex.
#### 10. thesis.pdf
This is the PDF file compiled by thesis.tex. No need to touch it as it will be updated by typesetting thesis.tex.
#### 11. thesis.tex
This is the most important file you will be editing with. I have created a lot of samples/examples in the template. If you have GUI, look into each sample sections/chapters, play with all the examples and understand how to modify them. For example, how can you insert a figure, table, a new chapter, an abbreviation or a reference?
##### --- Begin Document section
This part defines the frontpage and structure of your thesis. First fill the name, title, degrees, committee members, etc. It also defines the sequence of chapters (add more chapters based on your needs) where you write the thesis. Please follow the instructions!

### Final comment
Try search in Google, Stack Overflow/Exchange or overleaf if you find some LaTex functions or errors unclear. Again, I suggest a LaTex GUI which will save you a LOT of time in editing. Have fun with this template, and you'll find it much more efficient than MS Word when tuning the format of thesis.
