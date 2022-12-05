# Learning Java Through JShell

## Printing Hello World
Open a terminal, navigate to directory of this file, and invoke Java Shell.
```
jshell
```

Then type the following statment and press `enter` to print `Hello World` to the screen.
```
System.out.print("Hello World");
```

Exit JShell with the following command.
```
/exit
```

## Variables
Introduction to variables, keywords, and primative datatypes like `int`.

Make your first variable using the following command:
```
int myFirstNumber = 5;
```

Print out the value of the variable
```
System.out.print(myFirstNumber);
```

Change the value of the variable
```
myFirstNumber = 10;
```

## Starting out with Expressions
Expressions are the code to the right side of a declaration.
```
int myFirstNumber = (10 + 5) + (2 * 10);
```
`(10 + 5) + (2 * 10)` is the expression in the previous statement.

Create two new numbers for the rest of the lesson.
```
int mySecondNumber = 12;
int myThirdNumber = 6;
```

Verify the variables have been created succesfully with the following command:
```
/var
```
You should see the following output:
```
|    int myFirstNumber = 35
|    int mySecondNumber = 12
|    int myThirdNumber = 6
```

Now add the numbers together with one expression:
```
int myTotal = myFirstNumber + mySecondNumber + myThirdNumber;
```

## Decided to skip remaining lectures in First Steps Sections