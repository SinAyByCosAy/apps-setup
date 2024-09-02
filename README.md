## For MAC

Need to install homebrew(package manager)

```console
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

If the brew command is not found, put brew in the zshrc path.

```console
echo "export PATH=/opt/homebrew/bin:$PATH" >> ~/.zshrc
```

Clone the repo or download the mac-applications.txt file<br>
Go to the location of the file and run :

```console
xargs brew install --cask < mac-applications.txt
```

This will read all the list of applications from the file and pass them as arguments using the xargs utility.