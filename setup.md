# Setup and installation

## Dependencies
If you don't have it already you really should download [homebrew](https://brew.sh/) for managing packages on you mac.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
It's best to have [jenv](https://www.jenv.be/) installed on your system for managing your java environments.
```
brew install jenv
```
Follow the documentation to make sure you have jenv correctly added to your PATH.

## Install Java 17
This course is focussed most recently on the current LTS version of Java, Java 17.
To install the Java 17 jdk through homebrew run the following command
```
brew install openjdk@17
```

## Set Java 17 as JDK for Repository
Next you will want to set Java 17 as the JDK for the repository. To do this, navigate to root directory of this repository. First we need to add Java 17 to jenv. Do this with the following command.
```
jenv add ~/homebrew/opt/openjdk@17/libexec/openjdk.jdk/Contents/Home
```
If you installed the JDK manually or had homebrew install your JDK somewhere else, just specify the path to the `.jdk` file and add `/Contents/Home`.

Confirm that jenv has added the JDK to your list of versions witht he follwoing command.
```
jenv versions
```
You should see an item in the list that mentions openjdk 17.

Now that you've added the JDK to jenv we need to set Java 17 as the JDK for this project. To do that double check that you are still in the root directory of this repository, then run the following command.
```
jenv local openjdk64-17.0.5
```
If you downloaded a different minor version of the openjdk then specify the corresponding version number as defined by the the version from the `jenv versions` command.

Confirm that you've set the correct version by runing the following commands:
```
# Should output: openjdk....
jenv local
```
```
# Should output openjdk version "17.x.x" ...
java -version
```

And that's it. You should be ready to start programming in Java.