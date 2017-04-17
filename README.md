# Super basic note taker

Wanted something where I could take notes with ease and decided to write my own because
why not right?

Runs on top of `gvim` and `python3`. Those are the two deps for now. I'll try and make it
a little more compatible with other things in the future. 

Clone the repo or download the note file and copy it to your `/usr/local/bin` folder. Type
`note` to run the program. 

## What it does

All it does is create a file where the naming is based on the current date (so
YYYY-MM-DD.md). Yes, it's a markdown file. It then adds a timestamp entry as a secondary
heading and opens the file using gvim and places the cursor at the bottom of the file. If
you are making multiple notes for the day, you'll have multiple timestamps. That's all.

There's no find functionality. I search for stuff using grep. I might add some
functionality in the future to help with this which just rides on top of grep
