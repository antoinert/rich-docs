# Introduction

Rich is a Python library for writing rich text (with color and style) to the terminal, and for displaying advanced content such as tables, markdown, and syntax highlighted code.

Use Rich to make your command line applications visually appealing and present data in a more readable way. Rich can also be a useful debugging aid by pretty printing and syntax highlighting data structures.

## Requirements
Rich works with OSX, Linux and Windows.

On Windows both the (ancient) cmd.exe terminal is supported and the new Windows Terminal. The latter has much improved support for color and style.

Rich requires Python 3.6.1 and above. Note that Python 3.6.0 is not supported due to lack of support for methods on NamedTuples.

## Installation

You can install Rich from PyPI with pip or your favorite package manager:
<iframe title="card" style="border: 0;" width="100%" height="500px"
    src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=50d99d22-2b88-420a-a219-ce253e9d9ff6&collaborationId=KTDCJL63C3GITDX9"></iframe>

Add the -U switch to update to the current version, if Rich is already installed.

## Quick Start

The quickest way to get up and running with Rich is to import the alternative print function which takes the same arguments as the built-in print and may be used as a drop-in replacement.
You can then print strings or objects to the terminal in the usual way. Rich will do some basic syntax highlighting and format data structures to make them easier to read.

Strings may contain [Console Markup](https://rich.readthedocs.io/en/stable/markup.html#console-markup) which can be used to insert color and styles in to the output.

The following demonstrates both console markup and pretty formatting of Python objects:

<iframe title="card" style="border: 0;" width="100%" height="500px"
                        src="https://embed.tinnable.com/?recordId=403c003b-f442-40c2-a4bd-54260bfeffc0&cardId=70909b2d-6b66-4005-b918-fde59f057264&collaborationId=KTDCJL63C3GITDX9"></iframe>
