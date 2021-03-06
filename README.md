# Functionality

Mark lines in the editor and easily jump to them. _In Delphi style._
# Installation

Press `F1` in VSCode, type `ext install` and then look for `Numbered Bookmarks`.

# Usage

## Available commands

* **Numbered Bookmarks: Toggle Bookmark _'number'_** Mark/unmark the current line with a numbered bookmark
* **Numbered Bookmarks: Jump to Bookmark _'number'_** Move the cursor to the numbered bookmark
* **Numbered Bookmarks: List** List all bookmarks from the current file
* **Numbered Bookmarks: List from All Files** List all bookmarks from the all files
* **Numbered Bookmarks: Clear** remove all bookmarks from the current file
* **Numbered Bookmarks: Clear from All Files** remove all bookmarks from the all files

> Both **Toggle** and **Jump to Bookmark** commands are numbered from 1 to 9

![Commands](images/numbered-bookmarks-commands.png)

### Numbered Bookmarks: Toggle Bookmark _'number'_

You can easily Mark/Unmark bookmarks on any line. Works even for wrapped lines.

![Toggle](images/numbered-bookmarks-toggle.png)

> _new in version 0.2.0_  

### Numbered Bookmarks: List

List all bookmarks from the current file and easily navigate to any one. It shows you the line contents and temporarily scroll to that line.

![List](images/numbered-bookmarks-list.gif)

### Numbered Bookmarks: List from All Files

> _new in version 0.5.0_  

List all bookmarks from all files and easily navigate to any one. It shows you the line contents and temporarily scroll to that line.

![List](images/numbered-bookmarks-list-from-all-files.gif)

* Bookmarks from the active file only shows the line number and its contents
* Bookmarks from other files in the project also shows the relative path and filename
* Bookmarks from files outside the project are denoted with ![Folder](images/bookmarks-folder-icon.png)

## Available settings

> _new in version 0.4.0_  

* The bookmarks will be glued to the line of code _(context)_ instead of the line of the file
```
    "numberedBookmarks.useStickyBookmarks": true
```

![Sticky](images/numbered-bookmarks-sticky.gif)


* Allow bookmarks to be saved and restored, even if you close or change the Project
```
    "numberedBookmarks.saveBookmarksBetweenSessions": true
```

## Project and Session Based

The bookmarks are saved _per session_ for the project that you are using. You don't have to worry about closing files in _Working Files_. When you reopen the file, the bookmarks are restored.

It also works even if you only _preview_ a file (simple click in TreeView). You can put bookmarks in any file and when you preview it again, the bookmarks will be there.

# Changelog

## Version 0.5.2

* Tags added for Marketplace presentation

## Version 0.5.1

* **Fix:** Bookmarks becomes invalid when documents are modified outside VSCode

## Version 0.5.0

* **New Command:** List from all files
* **New Command:** Clear from all files

## Version 0.4.2

* **Fix:** Bookmarks missing in _Insider release 1.6.0_ (issue [#31](https://github.com/alefragnani/vscode-numbered-bookmarks/issues/11))

## Version 0.4.1

* **Fix:** Remove extension activation log (issue [#10](https://github.com/alefragnani/vscode-numbered-bookmarks/issues/10))

## Version 0.4.0

* **New Setting:** Sticky Bookmarks 

## Version 0.3.0

* **New:** Bookmarks are also rendered in the overview ruler
* **Fix:** Incompatibility with **Code February Release** 0.10.10 (issue [#4](https://github.com/alefragnani/vscode-numbered-bookmarks/issues/4))

## Version 0.2.0

* **New Command:** List all bookmarks from the current file

## Version 0.1.0

* Initial release

# Participate

If you have any idea, feel free to create issues and pull requests

# License

[MIT](LICENSE.md) &copy; Alessandro Fragnani

---

[![Paypal Donations](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=EP57F3B6FXKTU&lc=US&item_name=Alessandro%20Fragnani&item_number=vscode%20extensions&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted) a :coffee: if you enjoy using this extension :wink: