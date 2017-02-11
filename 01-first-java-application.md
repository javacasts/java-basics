Java Basics - First Java Application
====================================

> Java is a general-purpose computer programming language that is concurrent,
> class-based, object-oriented,[14] and specifically designed to have as few
> implementation dependencies as possible.
> - [Wikipedia](https%3A//en.wikipedia.org/wiki/Java_%28programming_language%29)

Setup
-----

So what do we need to program anything in Java?

 - Java Development Kit
 - Editor / IDE

How to install this depends on the system you are using. You can get the JDK
from [oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html).

Once installed, you should be able to call `java -version` and `javac -version`,
which would print out the version you've installed.

![`java -version`](java-version.png)

Then you need an editor. Source files are plain text-files, so you could use the
standard notepad in windows, but there are Integrated Development Environments
(IDE) available that help you write your code. Usually you would choose from
[Eclipse](https://eclipse.org/), [NetBeans](https://netbeans.org/), and
[IntelliJ IDEA](https://www.jetbrains.com/idea/), but you also can use
[Visual Studio Code](https://code.visualstudio.com/),
[Sublime](https://www.sublimetext.com/),
[emacs](https://www.gnu.org/software/emacs/), [vim](http://vim.org/) or any
other editor that can edit text-files.

Hello world
-----------

The first program in every language is usually a `hello world`-application. It
just prints out the message `hello world`. So, let's start wil the simpliest
`hello world` in java. Create a file with the name `HelloWorld.java`, and put
the following contents in there (using any editor).

``` java
class HelloWorld {

  public static void main(String[] args) {
    System.out.println("Hello world");
  }

}
```

So this is the source-code for the application. This first needs to be compiled
and then it can be executed.  
Java does not compile a standalone program, that would run on any machine, Java
uses a runtime that interprets the compiled Program. So here's what you need to
call:

``` sh
javac HelloWorld.java
java HelloWorld
```

This is how the outcome should look like:

![`hello world`](hello-world.png)
