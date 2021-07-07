# Proxy issue for vscode

Open up terminal by pressing `Ctrl + Backtick` on vscode.
When you execute following command in the terminal

```
dotnet run 
```

you might face the proxy issue with this error

```
Downloading package 'OmniSharp (.NET 4.6 / x64)' Failed at stage: downloadPackages Error: connect ETIMEDOUT 13.88.145.72:443
```

To fix it, press `Ctrl + Shift + P` to bring up the Command Palette then start typing "config" to filter and display the Configure Language Specific Setting command and open the settings.json file.
In the file, Click HTTP and you can see `"http.proxy: ",`. Set up your proxy and save and restart your vscode.
