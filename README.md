# useful-commands


* Find a list of last modified files in a directory
`find . -type f -print0 | xargs -0 stat --format '%Y :%y %n' | sort -nr | cut -d: -f2- | head`

