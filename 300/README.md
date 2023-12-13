# 300 - Building Our Application

Based on "NativeScript Tutorial for Beginners - Build iOS, Android and Web Apps with NativeScript" at https://www.youtube.com/watch?v=8Q8OtgL3Fuo

Run the following command from containers/app directory:

```
$ tns create HelloWorld --template nativescript-template-tutorial
```

If you receive an error like "No matching version found for nativescript-template-tutorial" just leave out the template option:

```
$ tns create HelloWorld
```

Without the template, you will be provided with alist of styles to choose from:

```
# Let’s create a NativeScript app!

Answer the following questions to help us build the right app for you. (Note: you
can skip this prompt next time using the --template option, or the --ng, --react, --vue, --svelte, --ts, or --js flags.)

? First, which style of NativeScript project would you like to use: › - Use arrow-keys. Return to submit.
❯   Angular - Learn more at https://nativescript.org/angular
    React
    Vue.js
    Svelte
    Plain TypeScript
    Plain JavaScript
```

This time we will choose **Svelte**. Point at it with your Up/Down keys and hit ENTER when on Svelte.

You will be informed as follows:

```
[@nativescript/webpack] Initialized config.
Project HelloWorld was successfully created.

Now you can navigate to your project with cd HelloWorld and then:

Run the project on multiple devices:

  $ ns run ios
  $ ns run android

Debug the project with Chrome DevTools:

  $ ns debug ios
  $ ns debug android

For more options consult the docs or run ns --help
```

Go into the new project directory:

```
$ cd HelloWorld
```

At any time you can run the ```tns help``` command to open the NativeScript CLI documentation in your browser.


MORE ...