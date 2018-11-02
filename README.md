# mpd_what
An mpd album art and info getter

mpd_what is a python script to grab album art and find out what is playing. In addition to finding art and info for what you're playing locally, it also will try to find art and info for internet radio stations you might be playing. Since every internet radio station is unique in its configuration, this script doesn't work with all of them, and maybe it never will, but it tries to do the best it can.

Getting started:

    pip3 install python-mpd2 pycurl musicbrainzngs python-magic
    
 * edit mpd_what to set the coverart_dir, mpd_host, and mpd_port to whatever you prefer (otherwise, it defaults to ~/coverart, localhost, and 6600, respectively)
    
    ./mpd_what -b

You can add a link to cover.jpg in your .conkyrc, or you can use `qiv --watch` to reload cover.jpg when it changes.
