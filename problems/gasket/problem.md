# gasket

This workshop teaches you how to use **command line modules** to process data.

The first module you will use is called **gasket**. You can install it like this:

```
npm install gasket -g
```

The **-g** puts a **gasket** command in your command-line path. If you get any
errors during installation try again with **sudo** or ask for help.

gasket simply runs commands for you, similar to Grunt, Gulp or Bash. Let's
start with something simple, a single **echo** command. We'll move on to some
non-trivial examples in later exercises.

gasket commands go in a **package.json** file under the **"gasket"** key, e.g.:

```
{
  "name": "my-module",
  "version": "0.0.1",
  "gasket": [
    "echo hi"
  ]
}
```

If you run **gasket** in the same folder as the above **package.json** file it
should simply print out **hi** to the console.

**To pass this challenge:**

Create a **package.json** file with a **"gasket"** section that prints out
**"hello world"** to the console.

Use the command **data-plumber verify package.json** to verify.
