# Chapter 2

## Rich Text
Rich has a Text class you can use to mark up strings with color and style attributes. You can use a Text instance anywhere a string is accepted, which gives you a lot of control over presentation.

You can consider this class to be like a string with marked up regions of text. Unlike a built-in str, a Text instance is mutable, and most methods operate in-place rather than returning a new instance.

One way to add a style to Text is the stylize() method which applies a style to a start and end offset. Here is an example:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=7ff1d08a-ab23-4bdd-a1a1-04123b15ab88&collaborationId=KTDCJL63C3GITDX9"></iframe>

This will print “Hello, World!” to the terminal, with the first word in bold magenta.

Alternatively, you can construct styled text by calling append() to add a string and style to the end of the Text.

If you would like to use text that is already formatted with ANSI codes, call from_ansi() to convert it to a Text object:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=c7dae8b6-315b-4ff1-bc52-85d7dddc9309&collaborationId=KTDCJL63C3GITDX9"></iframe>

Since building Text instances from parts is a common requirement, Rich offers assemble() which will combine strings or pairs of string and Style, and return a Text instance. The follow example is equivalent to the code above:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=1caa3ab2-74f6-43ec-889e-8d1c6183556b&collaborationId=KTDCJL63C3GITDX9"></iframe>

You can apply a style to given words in the text with highlight_words() or for ultimate control call highlight_regex() to highlight text matching a regular expression.

## Text attributes
The Text class has a number of parameters you can set on the constructor to modify how the text is displayed.

justify should be “left”, “center”, “right”, or “full”, and will override default justify behavior.

overflow should be “fold”, “crop”, or “ellipsis”, and will override default overflow.

no_wrap prevents wrapping if the text is longer then the available width.

tab_size Sets the number of characters in a tab.

A Text instance may be used in place of a plain string virtually everywhere in the Rich API, which gives you a lot of control in how text renders within other Rich renderables. For instance, the following example right aligns text within a Panel:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=90251c4b-036b-4291-bb13-655f959a19cc&collaborationId=KTDCJL63C3GITDX9"></iframe>
