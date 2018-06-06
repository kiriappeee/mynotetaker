# Super basic note taker

Wanted something where I could take notes with ease and decided to write my own because
why not right?

Needs `vi` and `python3` as the minimum dependencies to run. Other editors supported are
`vim`, `gvim`, and Visual Studio Code (`code`). To set a default editor, set the environment
variable `$EDITOR` to the editor of your choice.

eg: `export EDITOR=code` will open the note in VS Code

## To run

`wget https://raw.githubusercontent.com/kiriappeee/mynotetaker/master/note -O /usr/local/bin/note && chmod +x /usr/local/bin/note`

You might need `sudo` depending on the permissions of your `/usr/local/bin` directory.

**OR**:

Clone the repo/download the note file and copy it to a folder in your `$PATH`. Type
`note` to run the program. 

## What it does

It creates a directory called `~/.notes` and creates your markdown files in there.

All it does inside the notes directory is create a file where the naming is based on the current date (so
YYYY-MM-DD.md). Yes, it's a markdown file. It then adds a timestamp entry as a secondary
heading and opens the file using your editor and places the cursor at the bottom of the file. If
you are making multiple notes for the day, you'll have multiple timestamps. That's all.

There's no find functionality. I search for stuff using grep. I might add some
functionality in the future to help with this which just rides on top of grep

## Using it with Dropbox

I use this with my Dropbox. I've created a directory called `.notes` in my Dropbox directory and I run `ln -s /path/to/my/Dropbox/.notes $HOME`. Then whenever I create a note, it gets synced to Dropbox automatically. 
