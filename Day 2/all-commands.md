- `ls` list files in a directory
- `pwd` print working directory
- `cd` change directory
- `cd ..` change directory backwards
- `touch` create a file (if it doesn't exist)
- `mkdir` create a directory
- `cp` copy a file
- `rm` delete a file
- `mv` move a file (and or rename it)
- `head` see the first lines of a file or stream of text
- `tail` see the last lines of a file or stream of text
- `grep` return lines matching a string (or pattern)
- `cut` return a column or columns
- `sort` sort a file or stream
- `uniq` unique a list
- `nl` number lines of output
- `sed` edit a stream of text
- `which` see where a command is run from

## more complex things we did
- `head -n1000 GUTINDEX.ALL | tail -n5` return lines 995-1000
- `grep -i "Quixote\|Quijote" GUTINDEX.ALL -A3 | grep -B3 "Spanish"` find lines that contain *Quixote* or *Quijote* and are followed by a line containing Spanish up to two lines later
- `grep -i "German\|French" gutenberg.tsv | grep Shakespeare | awk '{print $NF}'` print the last field of lines which contain *French* or *German*
- `cut -f2 gutenberg.tsv | sort | uniq -c | sort -nr | head -n20 | nl` print and number the 20 most common authors in gutenberg.tsv
- `cut -f2 gutenberg.tsv | grep -i "jane austen" | sed 's/, January-March 1817//' | uniq -c` count the number of Austen titles, fixing one rogue string as we go
- `awk '{print $NF}'` print the last field of a file or stream (change to $1, $2 etc to get the first, second field of a file or stream, but `$NF` allows us to get the last field even when the number of fields varies between the lines). By default the delimiter for AWK is a tab.
- `echo $PATH` check what our path is
- `history | grep` check for what we did previously; for Mac you will need `history 0 | grep'`

Finally, here's the bash script, which you can save as something like `download-epub.sh` and run from the same directory with `bash ./download-epub.sh`:

```bash
#!/bin/bash
# download an ePub file from Gutenberg
# $1 = the Gutenberg ID
# $2 = the name of the downloaded epub, without termination
set -euo pipefail
curl -L0 https://www.gutenberg.org/ebooks/$1.epub3.images --output $2.epub`
```

Here's my solution to the exercise. There are many ways to do this, and you don't have to do it all in one line. In this solution I didn't try to take account of things like punctuation.


`cut -d" " -f1 paradise-lost.txt | grep "C" | sort | uniq -c | sort -n | tail -n 10 | awk '{print $NF}' > findlist.txt && grep -f findlist.txt paradise-lost.txt`
