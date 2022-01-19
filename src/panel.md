# Chapter 3

## Panel
To draw a border around text or other renderable, construct a Panel with the renderable as the first positional argument. Here’s an example:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=46cea22c-8dd7-4cd7-bdc2-710a827070d6&collaborationId=KTDCJL63C3GITDX9"></iframe>
                      
You can change the style of the panel by setting the box argument to the Panel constructor. See Box for a list of available box styles.

Panels will extend to the full width of the terminal. You can make panel fit the content by setting expand=False on the constructor, or by creating the Panel with fit(). For example:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=d6b5df08-50f2-4ba2-a1d2-f3f956315183&collaborationId=KTDCJL63C3GITDX9"></iframe>

The Panel constructor accepts a title argument which will draw a title on the top of the panel, as well as a subtitle argument which will draw a subtitle on the bottom of the panel:

<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=fc00d887-88f5-433c-863a-c05ba93b1303&collaborationId=KTDCJL63C3GITDX9"></iframe>

See Panel for details how to customize Panels.

## Rich Inspect
Rich has an inspect() function which can generate a report on any Python object. It is a fantastic debug aid, and a good example of the output that Rich can generate. Here is a simple example:

<iframe title="card" style="border: 0;" width="100%" height="500px"
                        src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=eb81f80d-d654-4a00-9516-e9f2759c6f4a&collaborationId=KTDCJL63C3GITDX9"></iframe>