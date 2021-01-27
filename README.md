# Python-On-Mac
Post Installation Configuration


If your default shell is sh (or possibly anything but bash) you won't be able to access your Anaconda python. If this is your case:

Go to Terminal/Preferences
Find 'Shells open with:'
Click the button for 'Command (complete path)'
Type /bin/bash as path
Restart your terminal. When you type $ which python you should now see the anaconda python. For me it was /Users/myname/anaconda3/bin/python.

$ echo $PATH will also change now to show to correct path, with anaconda first:

/Users/myname/anaconda3/bin:/Users/myname/anaconda3/condabin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Library/TeX/texbin:/opt/X11/bin

In Atom I had to add a shebang to the beginning of each script to set this as my preference: #!/Users/myname/anaconda3/bin/python
