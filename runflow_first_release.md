# We are happy to announce the first release of RunFlow, the new powerful efficiency tool

**RunFlow** is a cross-platform productivity tool which can launch apps and search files and more, that similar to [Wox](https://github.com/Wox-launcher/Wox) and [PowerToys](https://github.com/microsoft/PowerToys) on Windows, and also similar like [Alfred](https://www.alfredapp.com) and [Raycast](https://www.raycast.com) on macOS. But we have differences with these tools, and we have our own unique new features. Right now, at the below, we will introduce you what features of RunFlow have been implemented in more detail. It's an amazing journey, let's start.

### Cross Platform

The first main feature is cross-platform. Let you have a unified UI and operation experience when working cross-platform, do not need to switch tools.

> But Unfortunately for Linux users, the first edition of RunFlow have some fatal problems on Linux, so, currently, Linux is not supported yet. But we will try more efforts to fix these problems to make RunFlow working fine on Linux, and Linux will get support eventually.

### Multiple Languages

RunFlow support multiple languages, but by default, we only have english and simplified chinese. If you prefer to other languages, you can go to our [plugin store](https://myrest.top/store/plugin?query=language) to find a language translator, after you installed the plugin, you can choose your preferred language.

### Customizable Style and Theme

Here we want to introduce you one of our design philosophy is that we allow user to highly customize most thing, so we allow plugin to provide one or more window style and theme, to let you choose what you preferred.

### Triggered by Keyword

In RunFlow, a function must be provided by a keyword, unless some specials, such as language translator, theme provider and data sync service, etc. So likewise, a new keyword always mean a new function, and most of the plugins you installed also consist by keywords.

To use the function of the keyword, the most commonly way is just typing the keyword, if the function don't need any arguments, you can see the result row at the below, then to execute the result you can press `Enter` (ensure the result row is at the front, if not, you should press `Up` or `Down` to active it, or move mouse to hover on it) or double-click the result row.

![lock_computer](/local/myblog/images/lock_computer.png){width=70%}

If the function need one or more arguments, you should type a whitespace to separate the keyword and argument (multiple arguments also use whitespace to separate). For example, typing `timer start` to start a timer, the `timer` is a keyword, the `start` is an argument.

![timer_start](/local/myblog/images/timer_start.gif){width=70%}

However, if you input `start timer` is also work, is this case, `timer` is still the keyword, `start` is also still the argument, why this situation is ok?

Because we support the **`postfixed keyword`**, this feature allow you input the arguments first, input the keyword at last, this will be useful in some cases. For example, if you want to encode some literal by base64, you copied or dragged or typed the text as the argument first, but you forgot to type the keyword `base64` at the front, if we don't have the **`postfixed keyword`** feature, you must move cursor to the front, then type keyword `base64` and a whitespace to separate keyword and argument, fortunately, we have, you can just append the keyword after the text (also need a whitespace to separate), such as `myrest.top base64`.

any keyword

> Don't worry about these keywords you may think you should remember all of these keywords, we have a keyword suggestion function that can infer what you want to do by prefix matching. So you don't need to remember keywords, our `suggestion` will help you.

### Context Menu of Result

### Refreshable Result

### Toolbar

### Pinned Keyword

### Separate Window

### Hot Event

### Focused Mode

### Data Security and Synchronization

### Plugins

### Builtin Plugin
