# flash.sh

flashcards in your terminal!

This script is an expanded version of the one featured in [This nixcasts Video](https://www.youtube.com/watch?v=lX8jqo70r1I)

My expanded version will create a `flash` directory in `.local/share/` and create an empty `deck.csv` file for you.

You can have as many decks in the `flash` directory and having directories and nested directories filled with `.csv` decks will all work with this system.

Dependencies for this script are [fzf](https://github.com/junegunn/fzf) and [bat](https://github.com/sharkdp/bat).

To utilize this script copy/move it to your `~/.local/bin/` folder or any place in your `$PATH`

the `deck.csv` file should have colon `:` seperated values in 3 columns

Organized like this:

> `category:question:answer`

enjoy!
