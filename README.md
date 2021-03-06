# Node VGMusic Downloader

What is this ?
--------------

The Videogame Music Archive, also known as VGMusic.com or VGMA, is a website that archives MIDI sequences of video game music, ranging from tunes of the NES era to modern pieces featured in Xbox One, Wii U and PS4 games. Currently, there are over 30,000 MIDI sequences hosted on the site across approximately 47 gaming platforms. The SNES directory has the most MIDI sequences of any directory on this site. VGMusic.com is one of the oldest, if not the oldest, video game music websites online.

This tool will download all MIDI files listed on VGMusic.com.
This is for a personal use and must be considered as a disposable tool! Once you have all downloaded, please backup the files ;)

Default configuration will download files listed in all pages/categories. Download folder architecture follows the page URI's path.

Configuration
-------------

You can edit the `config.js` file in order to configure the script:

* `downloadFolder` is the download folder path (default: `./download`)
* `pages` is an array containing the list of pages/categories that will be crawled (default: all pages)
* There is a debug mode flag (default: off)

How to use
----------

You must have Node.js installed on your computer.

1. Git clone, or download zip file
2. Install dependancies using `npm install`
3. Edit the configuration file `config.js` if needed
3. Run the app with `node vgmusic.js` !

How to monitor crawling ?
-------------------------

Two nice commands to see what's going on when the script is running : 

* `du -sh ./download` displays the total size of what you crawled
* `find ./download -name "*.mid" | wc -l` count the number of MIDI files you downloaded
