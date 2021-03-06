# Colab (Google Drive) notebooks

Google now allows you to create Python notebooks within Google Drive.

To do this, make sure you are logged in to Google Drive and go to [https://colab.research.google.com/](https://colab.research.google.com/).

A window should appear with various tabs. At the bottom right of the window you can [create a **NEW PYTHON 3 NOTEBOOK**](https://colab.research.google.com/notebook#create=true&language=python3).

Click this.

## The different elements in a Pythonnotebook

The file will be called something like *Untitled0.ipynb*. It's worth outlining the different elements on the page in turn:

* **File name** (*Untitled0.ipynb*): you can double-click on the name to rename it, like any other Google document. Note the `ipynb` extension which indicates it is a Python notebook.
* **Menus**: the notebook has 7 menus, from *File* to *Help*. You can use these to export your notebook as pure Python script, bring up shortcuts and look at the code in different ways, among other things.
* **+ CODE** and **+ TEXT** buttons: click on one of these to create a new section of code in your notebook, or a new section of text (at the moment the document has one empty code section)
* The **notebook itself**, which takes up most of the screen. This current consists of a line of empty code at the top of the document.

## Creating and formatting text in a notebook

Click on the **+ TEXT** button to create a new text section in your notebook. This will be inserted at the bottom, underneath the empty code section. The cursor will already be flashing, so you can start typing (if it is not, just double-click to edit a text section). 

Type into the text box: "Above is a line of code"

Note that there are formatting buttons just above the text. These include:

* A heading button
* Bold
* Italic
* Linking
* Insert image
* Indent
* A numbered or bullet list
* A horizontal rule 

One which needs a bit more explanation is the  `<>` button. This allows you to *format* text as 'code'. In other words, it will make text a different font, so that it looks like this: `print("hello")`.

That text will not be *working* code, however: it will not run or do anything. 

**Have a play with the formatting buttons** and see what they do to your text. You will notice the following:

* Making something a heading will add a `#` to the start of the line. If you click it twice you will get `##` for a second level heading (subheading), and three times will give you `###` for a third level heading (sub-subheading).
* Making something bold will add `**` before and after the bold text
* Making something italic will add `*` before and after the bold text
* Adding a link will put the linked text inside square brackets, and the URL inside round brackets immediately after

Other formatting will add different characters too. 

Those characters are **Markdown**. This is a simple language for adding formatting to text in the same way you might use HTML tags such as `<b>` to make text bold.

You can use Markdown in your text directly, too. Try typing the same special characters (e.g. asterisks immediately before and after words to make them bold and/or italic) to format text without having to use the buttons.

Notice also that, while you are typing in it, the text section is split into two columns: the typing is done on the left but to the right is an area which shows a *preview* of how your text looks. That preview does *not* include the Markdown - only the resulting text once the formatting has been applied. 

When you click away from the text box (for example, click on the code section instead), you will notice you now can just see the formatted version of the text. 

To return to the editing view, just double-click that section at any time.

## Moving sections

At the moment our text section is below the code section, but we would really prefer it to come *before* the code. That's a good excuse to introduce some other options...

Click on the text section and look in the upper-right corner: there should be some more buttons there which allow you to:

* Move the section up or down
* Get a link which will take someone directly to that section
* Add a comment to the section
* Edit the section
* Delete the section
* Access more options, including copying or cutting the section

Use these options to move the text section to the top of the document.

Now it's time to turn our attention to the code section.

## Writing and running code in a notebook

Every new notebook has one code section by default, so we already have a code section in the notebook. This can be edited by simply clicking into it (you don't have to double-click).

Click into your code section and write the following:

```py
print("hello")
```

Then click the 'play' button (actually it means 'run') to the left of that section.

The code in that section will now run. Two things to point out here:

1. A number in square brackets will appear to the left of the code section. This indicates the order in which a section of code has been run, so at the moment this will be `[1]` to indicate that this was run first. If sections of code have been run out of sequence (for example a section at the bottom of a notebook was run first, and then one near the top), these numbers can help you to identify that. It will also indicate if code has been run and then deleted (numbers will be missing).
2. Any **output** from the code will be displayed underneath the code section. Sometimes - in fact, often - code will not have any obvious output. The `print()` command above is often used to create an output that allows us to see what's happening inside the code. But unless we ask it to show us in this way, we won't necessarily be able to check what the code is doing.

To demonstrate this, create a new code section and type the following:

```py
myname = "Paul"
```

And *run* the code.

Note that this time there is no output. 

What you have done with that line of code is create a new **variable**. A variable is a way to store information in code. In this case it is storing the text `"Paul"`.

If we want to check what is in that variable, we can use `print()` again, this time putting the variable name inside the brackets:


```py
print(myname)
```

Now we can see the *contents* of that variable. 

Some other things to point out about this variable. You will notice that `"Paul"` was in quotation marks. This tells Python that we are storing text (in programming, what we call a **string**: a string of characters).

If we didn't use quotation marks... 

```py
myname = Paul
```

...we would get an error:

`NameError: name 'Paul' is not defined`

This is because Python now assumes we are referring not to a string of characters "Paul", but instead that `Paul` means something special. For example, it might be the name of a command, or another variable, or a piece of code called a function. 

