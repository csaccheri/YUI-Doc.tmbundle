JS Lint? Check.  
Unit tests? Check.  
Documentation? Umm...  

Don't worry -- documenting your JavaScript can be fun and easy! (Well, maybe just easy.)
 
This bundle provides tools for running and writing comments with [YUI Doc][ydoc] directly from TextMate. YUI Doc is a great application for automatically generating documentation from commented JavaScript source code.

## Installation

Install from Github:

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles
    cd ~/Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/csaccheri/YUI-Doc.tmbundle.git "YUI Doc.tmbundle"
    osascript -e 'tell app "TextMate" to reload bundles'

Or use [GetBundles][getb] (search for "YUI Doc").

**Important!** YUI Doc itself relies on Python and four external libraries; these must be installed before running YUI Doc. [Follow these setup instructions.][ydop]

## Usage

### Snippets

This bundle includes a number of snippets to help you write YUI Doc-friendly comments. Use the `docblock` snippet (type `doc` then tab) to create a documentation comment block (starting with `/**`), then use the other snippets to generate the various tags YUI Doc supports.

Read the [YUI Doc tag reference][ydop] for a description of each tag and how it's used.

### Commands

* **Document with YUI Doc** (⌃⌘D)
Generates HTML documentation from commented JavaScript source code using YUI Doc 1.0.0b1 and displays it in TextMate's Web Preview window. Select a directory (or multiple directories) to document and then run the command. If no directories are selected, the command will generate documentation for all JS files in the project drawer.

* **View Tag Reference** (⌃⌘D)
Opens the [YUI Doc tag reference][ydot] in TextMate's Web Preview window.

## License

* **[YUI Doc][ydoc]** ([BSD License][bsd])

[bsd]:    http://yuilibrary.com/license/
[ydoc]:   http://developer.yahoo.com/yui/yuidoc/
[ydop]:   http://developer.yahoo.com/yui/yuidoc/#start
[ydot]:   http://developer.yahoo.com/yui/yuidoc/#tags
[getb]:   http://svn.textmate.org/trunk/Review/Bundles/GetBundles.tmbundle/