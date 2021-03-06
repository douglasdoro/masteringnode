# Mastering Node

 Mastering node is an open source eBook by node hackers for node hackers. TJ started this as a side project and realized that he didn't have time :) Jim picked up some editing and project structuring.  It's open to everyone, so go nuts, download it, build it, fork it, extend it and share it. If you come up with something you wish to contribute back, send a pull request.

## Authors

 - TJ Holowaychuk ([visionmedia](http://github.com/visionmedia))
 - Jim Schubert ([jimschubert](http://github.com/jimschubert))

## Formats

 Mastering node is written using the markdown files provided in `./chapters`, which can then be converted to several output formats, currently including _pdf_, _mobi_, _epub_ and of course _html_.

## All Formats

    $ make

## PDF

Required by `make book.pdf`:

    $ brew install htmldoc
    $ make book.pdf

## HTML

Required by `make book.html`:

Node.js is required to convert markdown to html.  The conversion process was borrowed from node.js and its generation of API documentation.

The scripts are located in tools/docbook with minor modifications from the node.js repository.

    $ make book.html

## EPUB

Required by `make book.epub`:
Requires [Calibre](http://calibre-ebook.com/)

    $ make book.epub

## MOBI

Required by `make book.mobi`:
Requires [Calibre](http://calibre-ebook.com/), specifically `ebook-convert` version 3.

To install the most recent version of calibre:

    sudo python -c "import urllib2; exec urllib2.urlopen('http://status.calibre-ebook.com/linux_installer').read(); main()"

To make the `book.mobi` format:

    $ make book.mobi

## References

Contents of this eBook currently reference the following software versions:

  - node 0.4.0

## Source

All example source can be run simply by executing node against the file,
for example:

      $ node src/events/basic.js

## Hacking node

Executing node without parameters will enter a node console, a Read-Eval-Print-Loop (REPL). Here, you can inspect objects and execute commands.

	> require
	{ [Function: require]
	  resolve: [Function],
	  paths: 
	   [ '/home/jim/.node_modules',
	     '/home/jim/.node_libraries',
	     '/usr/local/lib/node' ],
	  main: undefined,
	  extensions: { '.js': [Function], '.node': [Function] },
	  registerExtension: [Function],
	  cache: {} }
	> console
	{ log: [Function],
	  info: [Function],
	  warn: [Function],
	  error: [Function],
	  dir: [Function],
	  time: [Function],
	  timeEnd: [Function],
	  trace: [Function],
	  assert: [Function] }
	> 


## License

Node.js is an official trademark of Joyent. This work is not formally related to or endorsed by the official Joyent Node.js open source or commercial project.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://creativecommons.org/images/public/somerights20.png" /></a><br /><span xmlns:dc="http://purl.org/dc/elements/1.1/" href="http://purl.org/dc/dcmitype/Text" property="dc:title" rel="dc:type">Mastering Node</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">TJ Holowaychuk</span> is licensed under a <br/> <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/">Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License</a>.
