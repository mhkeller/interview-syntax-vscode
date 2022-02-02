Interview Syntax
===

A VS Code syntax definition and highlighter meant to help reporters as they conduct interviews.

Using [Markdown](http://dillinger.io/) as a jumping off point, Interview highlights whether certain parts of the conversation are on the record, on background or off the record.

It looks best with the [Spacegray Eighties](http://github.com/mhkeller/outer-spacegray-vscode) theme. It will work in other color schemes as long as they have markdown styles but its aesthetics are not guaranteed.

## Who's it for

If you're a reporter who does some programming in VS Code, this can be a useful tool to give more structure and verifiability to interviews you conduct.

If you're a reporter who doesn't program, it can perform the above but also be a useful starting point to familiarize yourself with a text editor.

## What it looks like

Here's an example:

![](https://raw.githubusercontent.com/mhkeller/interview-syntax-vscode/master/assets/example-interview.png)

## How to use it

Save your files as `.interview` or `.vw` and VS Code should handle the rest. It also comes with a handy snippet that will give you an interview template by typing `interview` and then hitting the <kbd>tab</kbd> key, which will give you a file that looks like the example below.

![](https://raw.githubusercontent.com/mhkeller/interview-syntax-vscode/master/assets/start-interview.gif)

### Styling for on the record, on background or off the record

Generally, the interview has ground rule terms for how the person wants to be attributed. Interviews can get tricky, however, when the interviewee jumps back and forth. As shown in the screenshot above, you can highlight different regions by surrounding them with tick marks ( \` ) and adding either the `on`, `bg` or `off` keywords.

```
`on
This is on the record
`

`bg
This is on background
`

`off
This is off the record
`
```

### Export to Word document

If you install Pandoc, you can also automatically convert your `.interview` files into Word documents by running <kbd>shift</kbd> <kbd>cmd</kbd> + <kbd>b</kbd>. The output doesn't handle single line breaks super well so if you're exporting, you might want to add an extra line break between lines of text.

You can install pandoc from its [GitHub page](https://github.com/jgm/pandoc/releases/tag/1.13.2). Scroll all the way to the bottom to select your operating system. Or, if you have [homebrew](http://brew.sh) installed, you can run `brew install pandoc`.

### Shortcuts

###### Template - `interview` + <kbd>tab</kbd>

This will prefill your page with the interview template pictured above.

###### Questions — <kbd>cmd</kbd> + <kbd>?</kbd>

This will start a question for you by writing out `// `. This is useful if you think of a question or note to yourself mid-interview. You can turn turn an existing line into a question with this shortcut as well.

###### Block comments — <kbd>option</kbd> <kbd>cmd</kbd> + <kbd>?</kbd>

This will start a block comment (a comment that spans mutliple lines) by writing out `/* */` and placing your cursor in the middle. Same as the question shortcut, you can highlight multiple lines and turn them into a comment block with this shortcut.

###### Spell check — <kbd>F6</kbd>

This is a general Sublime Text shortcut and is enbaled by default for `interview` files. If it doesn't load, on a Macbook, trigger this by holding down the <kbd>fn</kbd> key before pressing <kbd>F6</kbd>, otherwise it will just change the keyboard brightness.

## Installation

Copy the files in the `Interview` folder into your VS Code user packages directory. Open this directory by going to the menu bar `Sublime Text > Preferences... > Browse Packages...` and then open the `User` foler.

## Contributing

If you want to help that would be greatly appreciated! 

### Other formatting

Here's an example of the other types of formatting you can use.

![](https://raw.githubusercontent.com/mhkeller/interview-syntax-vscode/master/assets/all-formatting.png)
