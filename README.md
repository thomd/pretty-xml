Pretty-XML &mdash; Prettify a XML file
======================================

A ruby gem which does &mdash; for the time being &mdash; only one thing: format a XML file.

Generated XML files are often poorly formatted. Use the `xmlfo` command to properly indent and normalize the file. It will output the XML with consistent indenting, based upon the logical nesting depth of the tags.

Installation
------------

Use [jewelers][1] build in functionality to generate `*.gemspec` files and install gem with

    rake gemspec
    sudo rake install
    
Check `rake -T` for more commands.

Use [rocco][2] for generating a rocco-prepared documentation of the `xmlfo` script:

    rokko bin/xmlfo
    
Usage
-----

Format _all_ xml-files found within the current directory and append a _default_-postfix `_fo` (as an abreviation of _formatted_) to the output filename  
(e.g. a file _input.xml_ becomes _input_fo.xml_):

    xmlfo -a

Format _all_ xml-files found within the current directory and append a postfix `_postfix` to the output filename  
(e.g. a file _input.xml_ becomes _input_postfix.xml_):

    xmlfo -a -p postfix
    xmlfo -ap postfix

Format the file _input.xml_ only and append the default-postfix `_fo` to the output filename:

    xmlfo <input.xml>

Format the file _input.xml_ only and append a postfix `_postfix` to the output filename:

    xmlfo -p postfix <input.xml>
    


    
[1]: http://github.com/technicalpickles/jeweler  "Jeweler at Github"
[2]: http://rtomayko.github.com/rocco/  "Rocco at Github"

