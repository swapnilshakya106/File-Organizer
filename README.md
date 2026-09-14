# File-Organizer
A Python CLI tool that automatically organizes files in a folder into subfolders by type (images, documents, music, code, etc.)

#File Organizer 

A simple Python command-line tool that automatically organizes messy folders (like your Downloads folder) by sorting files into subfolders based on their file type.

How it works

Give it a folder path, and it will:

1.Scan every file directly inside that folder
2.Detect each file's type (image, document, music, video, code, etc.)
3.Move it into a matching subfolder (creating the subfolder if it doesn't exist)

Example

Before:

Downloads/
    photo.jpg
    resume.pdf
    song.mp3
    notes.txt
    script.py

 
 After running the script:

Downloads/
    Images/photo.jpg
    Documents/resume.pdf
    Music/song.mp3
    Text Files/notes.txt
    Code/script.py

 File categories
Category	Extensions
Images =	.jpg, .jpeg, .png, .gif, .webp, .svg
Documents	= .pdf, .doc, .docx, .xls, .xlsx, .ppt, .pptx
Text Files =	.txt, .md, .csv
Music =	.mp3, .wav, .m4a
Videos =	.mp4, .mkv, .mov, .avi
Archives =	.zip, .rar, .7z, .tar, .gz
Code =	.py, .js, .html, .css, .java, .cpp
Others 	anything not listed above   

You can easily add more file types by editing the FILE_TYPES dictionary at the top of the script.

How to run ?

Write in a terminal

bash : python file_organizer.py


It will ask for the full path of the folder you want to organize, then sort it automatically.

Concepts used
______________

1.File handling with the os module (os.listdir, os.path.splitext, os.makedirs)
2.Moving files with shutil.move
3.Dictionaries for mapping extensions to categories
4.Functions and a simple command-line interface

Why this project ?

Sorting downloaded files by hand gets tedious — this is a small, genuinely useful automation script and a good example of using Python for everyday tasks, not just algorithms.

Made by Swapnil while learning Python 😄
