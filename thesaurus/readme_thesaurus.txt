        
                                                *'thesaurus'* *'tsr'*
'thesaurus' 'tsr'       string  (default "") 
                        global or local to buffer |global-local|
        List of file names, separated by commas, that are used to lookup words
        for thesaurus completion commands |i_CTRL-X_CTRL-T|.
        
        Each line in the file should contain words with similar meaning,
        separated by non-keyword characters (white space is preferred). 
        Maximum line length is 510 bytes. 
        
        An English word list was added to this github issue:
        https://github.com/vim/vim/issues/629#issuecomment-443293282
        Unpack thesaurus_pkg.zip, put the thesaurus.txt file somewhere, e.g.
        ~/.vim/thesaurus/english.txt, and the 'thesaurus' option to this file
        name.

        To include a comma in a file name precede it with a backslash.  Spaces
        after a comma are ignored, otherwise spaces are included in the file
        name.  See |option-backslash| about using backslashes.
        The use of |:set+=| and |:set-=| is preferred when adding or removing
        directories from the list.  This avoids problems when a future version
        uses another default.
        Backticks cannot be used in this option for security reasons.

