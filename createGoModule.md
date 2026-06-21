# Tutorial: Create a Go module
This is the first part of a tutorial that introduces a few fundamental features of Go language. If you're just getting started with Go, be sure to take a look at [Tutorial: Get started with Go](https://go.dev/doc/tutorial/getting-started.html), which introduces the go command, Go modules, and very simple Go code.<br>

In this tutorial you'll create two modules. The first is a library which is intended to be imported by other libraries or applicaitons. The second is a caller application which will use the first.<br>

This tutorial's sequence includes seven brief topics that each illustrate a different part of the language.
1. Create a module -- Write a smal module with functions you can call from another module.
2. [Call your code from another module](#Call-your-code-from-another-module) -- IMport and use your module.
3. [Return and handle error](#return-and-handle-an-error) -- Add a simple error handling.
4. [Return a random greeting](#return-a-random-greeting) -- Handle data in slices (Go's dynamically-sized arrays).
5. [Return greetings for multiple people](#return-greetings-for-multiple-people) -- Store key/value pairs in a map. 
6. [Add a test](#add-a-test) -- Use Gos's built-in unit testing features to test your code. 
7. [Compile and install the application](#compile-and-install-the-application) -- Compile and install your code locally.

### Prerequisites
* **Some programming experience.** The code here is pretty simple, but it helps to know something about functions, loops, and arrays.
* **A tool to edit your code.** Any text editor you have will work fine. Most text editors have good support for Go. The most popular are VSCode (free), GoLand (paid), and Vim (free).
* **A command terminal.** Go works well using any terminal on Linux and Mac, and on PowerShell or cmd in Windows.

### Start a module that others can use
Start by creating a Go module. In a module, you collect one or more related packages for a discrete and useful set of functions. For example, you might create a module with packages that have functions for doing financial analysis so that others writing financial analysis can use your work.
<br>
Go code is grouped into packages, and packages are grouped into modules. Your module specifies dependencies needed to run your code, including the Go version and the set of other modules it requires.
<br>
As you add or improve functionality in your module, you publish new versions of the module. Developers writing code that calls functions in your module can import the module's  updated packages and test the new version before putting into production use. 
1. Open a command prompt and cd to your home directory. 
On Linux or Mac:
```bash
cd
```

## Create a module

## Call your code from another module
In the [previous section](#create-a-module), you created a greetings module.
