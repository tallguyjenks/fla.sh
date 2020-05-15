<!-- Header & Preview Image -->
<h1 align="center">
<img src="/img/flashheader.png" height="50%" width="50%">
</h1>

<!-- Shields -->
<p align="center">
<a href="https://github.com/tallguyjenks/fla.sh/blob/master/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=flat&label=License&message=MIT&logoColor=eceff4&logo=github&colorA=black&colorB=green"/></a>
<a href="https://img.shields.io/travis/tallguyjenks/fla.sh/master"><img src="https://img.shields.io/travis/tallguyjenks/fla.sh/master"></a>
<img src="https://img.shields.io/github/commit-activity/m/tallguyjenks/fla.sh">
<a href="https://github.com/tallguyjenks/fla.sh/graphs/contributors"><img src="https://img.shields.io/github/contributors/tallguyjenks/fla.sh"></a>
<img src="https://img.shields.io/github/v/release/tallguyjenks/fla.sh">
</p>

<!-- Description -->
> flashcards in your terminal! This script was inspired by a basic script i saw in a youtube video by a user named nixcasts. I Like the Anki flashcard system and so im working to replicate it in a simple manner using plain text documents and a shell script to aid my ability to study with active recall and spaced repetition.

![Preview of fla.sh](./img/flash_preview.png)

This script is an expanded version of the one featured in [This nixcasts Video](https://www.youtube.com/watch?v=lX8jqo70r1I)

This expanded version will create a `flash` directory in `.local/share/` and create an example `deck.csv` file for you.

You can have as many 'decks' in the `flash` directory as you want, and having directories and nested directories filled with `.csv` 'decks' will all work with this system. There is also no practical limit on the amount of 'cards' a 'deck' can hold.

## Dependencies

This script uses:

- [fzf](https://github.com/junegunn/fzf)
- [bat](https://github.com/sharkdp/bat) (optional if you use `flash -p cat` to use the core utility instead of `bat`)
- (if on macOS the GNU core utilities are a dependency (namely the `shuf` utility))

Install these prior to running the script.

## Installation

### Windows

Untested, not sure if this script and its dependencies will work with WSL or not.

### Mac

Will need to have `brew` to install dependencies listed below and also `brew install coreutils` to get the GNU core utilities as `shuf` is not in macOS by default.

You will need to put the script itself somewhere in your `$PATH` and execute it to initialize setup.

Confirmed to work on macOS 10.14.6 more recent version welcome to test and file an issue/pull request to update README if other versions run the script as it should.

### Linux

To utilize this script copy/move it to your `~/.local/bin/` folder or any place in your `$PATH`

## Troubleshooting

> Common issues will be added here as they arise during the stability stage of this script.

Checks:

- Is your system supported? see above
- Are all necessary dependencies installed?
- what version of bash do you have installed? or do you have bash installed?

## Usage

The `deck.csv` file should have colon `:` separated values in 4 columns

Organized like this:

> `category:question:answer:0`

**First Field:** _The category of the flashcard_

**Second Field:** _The Question being asked_

**Third Field:** _The Hidden Answer_

**Fourth Field:** _The Score*_

> \* The score determines how often which cards are shown to you. A good idea is to start all your cards out at 0 so they are all served to you equally. As you study and review and mark the more familiar cards as 'Mild' or 'Easy' more points will be added. The lower point cards are sorted to the top and the top 10 are taken and shuffled and then drawn from. This way as you learn the material the items you are less familiar with bubble up into the shuffled pool for drawing and those that go up in points due to increased familiarity go down because you're rating the material as easier.

### Decks

If you would like to browse a collection of decks readily available in your subject matter that are comaptible with [fla.sh](https://github.com/tallguyjenks/fla.sh) then you should check out [Flash Decks](https://github.com/tallguyjenks/Flash-Decks).

## Media (accepting contributions)

- [Fla.sh Plain Text Flashcards in your Terminal](https://www.youtube.com/watch?v=DbakjEAc_MU)
- [Flash Cards In Your Terminal With Fla.sh](https://www.youtube.com/watch?v=KEWhOzDCfLg)
- [Fla.sh++ A Comprehensive Walk Through of My Bash Flashcard Script Project](https://www.youtube.com/watch?v=nPNPXEh6BUA)
- [Even Exam Prep Can Be Done From The Terminal With Fla.sh](https://www.youtube.com/watch?v=RJ094P7wxaU)


## Support

This is free, open-source software. If you'd like to support the development of future projects, or say thanks for this one, you can donate to me through [paypal](https://www.paypal.me/tallguyjenks) or buy me a coffee:

<!-- Buy me a coffee -->
<h3 align="center">
<a href="https://www.buymeacoffee.com/tallguyjenks" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
</h3>
<!-- Footer Image -->
<h3 align="center">
<img src="/img/flashfooter.png">
</h3>

