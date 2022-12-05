# IntelliJ Basics

## Install IntelliJ
Navigate to the downloads page: https://www.jetbrains.com/idea/download/ and follow installation wizard

## Configuring IntelliJ
Need to tell IntelliJ what JDK to use and where it is. If you installed the JDK through homebrew it should be at this path:
```
~/homebrew/opt/openjdk@17/libexec/openjdk.jdk
```

Navigate to Settings or Preferences and go to Editor > General > Auto Import and select the check box next to 'Add unambiguous imports on the fly' and 'Optimize imports on the fly'

To better see what is happening and what is required in the source code navigate to Code Folding and unselect 'File header', 'Imports', 'One-line methods', 'Closures', and 'Generic constructor and method parameters'