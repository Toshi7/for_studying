Using GitHub with Visual Studio
=====================================


Reference
------------------------------
- [Step by Step working with GitHub Repository and Visual Studio 2015](http://www.infragistics.com/community/blogs/dhananjay_kumar/archive/2016/07/21/step-by-step-working-with-github-repository-and-visual-studio-2015.aspx)
- [Using GitHub with Visual Studio 2012 / 2013 / 2015](https://www.youtube.com/watch?v=Ijfypw7qJgg)

while pusing the code to GitHub, I get this error message below
```
Error encountered while pushing to the remote repository: Git failed with a fatal error.
fatal: unable to access 'https://github.com/Toshi7/practice_.Net_Core.git/': Failed to connect to proxy.occ.co.jp.com port 8080: Connection refused
Pushing to https://github.com/Toshi7/practice_.Net_Core.git
```

To fix it, you need to go to C:\Users\[your username]\.gitconfig
```
[http]  
    proxy = http://yourproxy.com:8080  //change your settings here
[https] 
    proxy = http://yourproxy.com:8080  //change your settings here
```

Reference [Failed to connect to github 443](http://stackoverflow.com/questions/29333319/failed-to-connect-to-github-443)
