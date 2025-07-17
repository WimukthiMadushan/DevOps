**DevOps** is a modern approach that combines **development** and **operations** to build, test, and release software **faster and more reliably**. It focuses on **collaboration, automation, and continuous improvement**, helping teams deliver better products with **speed, efficiency, and stability**. DevOps bridges the gap between coders and IT teams, turning ideas into real-world solutions quickly.

## 📘 Linux Skills Overview

- 🖥️ Learn how to interact with the terminal and understand the shell, the gateway to the Linux kernel.
- ⚙️ Study core Linux concepts that help you understand how systems operate.
- 📦 Explore various package management methods used by different Linux distributions.
- 🧭 Gain confidence in navigating the command line, manipulating files, and using a variety of text editors.
- 🔐 Understand file-level security, configure permissions, and implement essential Linux security practices.
- 🌐 Troubleshoot networking connectivity issues effectively.
- 💽 Configure storage options including disk formatting, mounting, and creating logical volume groups.
- 🚀 Set up custom applications to start on boot using **SYSTEMD**, the primary initializer for Linux services.

  Basic Linux Commands

The top-level directory (/home/Michael) already exists since it is Michael’s home directory. You will create subdirectories inside it manually. In this exercise, we create four continent directories (Asia, Europe, Africa, and America) under /home/Michael. Under each continent, country directories and for some, city directories are added. Each bullet point in the description below represents a directory.

When you log in as the user Michael, your starting point is the home directory (/home/Michael). 

```
pwd
/home/michael
ls
(Desktop Downloads Pictures ...)
```

Creating Directories

```
mkdir Asia Europe Africa America
```

Absolute vs. Relative Paths

When moving around the file system, you have two options: absolute paths and relative paths. For example, if you're in /home/Michael and want to navigate to the Asia directory:

```
cd /home/Michael/Asia   (Absolute Path)
cd Asia                 (Relative Path)
```

An absolute path begins from the root directory (/) and provides the full location, whereas a relative path is based on your current working directory.

Moving Directories

To relocate the Morocco directory from Europe to Africa, use the mv command. When using absolute paths:

```
mv /home/michael/Europe/Morocco /home/michael/Africa/
```

Renaming Directories
```
mv Asia/India/Mumbai Asia/India/MumbaiCorrected
```

Copying Files
To copy the city.txt file from the Mumbai directory to the Cairo directory (located in Africa/Egypt), use:
```
cp Asia/India/Mumbai/City.txt Africa/Egypt/Cairo/
```
Deleting Files
```
rm Europe/UnitedKingdom/London/Tottenham.txt
```

## Working with Files

Reading File Contents

To display the contents of a file—such as city.txt in the Mumbai directory—use the cat command:

```
cat Asia/India/Mumbai/City.txt
```

Writing to Files

To replace the content of a file, like updating the Cairo version of city.txt, use redirection with cat:
```
cat > Africa/Egypt/Cairo/City.txt
```
After executing the command, type the new content. Press Ctrl+D when finished to save and exit.

Creating an Empty File

To create an empty file—such as country.txt in the China directory—use the touch command:
```
touch /home/michael/Asia/China/Country.txt
```

Viewing Files with Pagers.

For a more manageable view of file contents, you can use pagers like more and less.

more new_file.txt

Key controls for more:

Space: scrolls one screen.
Enter: scrolls one line.
b: scrolls back one full screen.
/: begins a text search.
q: quits the viewer.

Using less offers additional navigation controls:
```
less new_file.txt
```
Key controls for less:

Up Arrow: scrolls up one line.
Down Arrow: scrolls down one line.
/: begins a text search.
q: quits the viewer.


More powerful text editors are available for advanced file manipulation and will be covered in a dedicated section later.

Listing Files

The ls command lists the contents of directories. For a basic listing, use:
```
ls
```

For a detailed view showing file permissions, ownership, and timestamps, add the -l option:
```
ls -l
```
Example output:
total 0
```
-rw-rw-r-- 1 bob bob 0 Mar 13 11:30 File.txt
-rw-rw-r-- 1 bob bob 0 Mar 13 11:30 index.html
-rw-rw-r-- 1 bob bob 0 Mar 13 11:30 caleston
```

To include hidden files (those starting with a dot), use:
```
ls -a
```

Example output:

.  ..  File.txt  index.html  caleston  .test
Here, . refers to the current directory and .. to the parent directory.

To sort files by modification time (newest first), use:
```
ls -lt
```

For a list from oldest to newest, use:
```
ls -ltr
```

This guide covered fundamental Linux commands for effectively navigating and manipulating your file system. With these basics, you can work more efficiently and manage your directories and files with ease.






