# node-cgi

Node module to call node scripts as CGI scripts

# USAGE

#!/usr/bin/node
var cgi = require('node-cgi');
var param = cgi.getParameters();
cgi.print("Hello world<br/>\n");
cgi.print("parameters="+require('util').inspect(params)+"<br/>\n");


# FEATURES

* A node script can be called from Apache by giving it the .cgi extension and making it executable
* Supports GET as well as POST () parameters
* Can set a custom mimetype with cgi.getParameters() (default text/html)
* Can include a script relative to the current script with eval(cgi.read('path/to/relativ/script.js'))

# LICENSE

node-cgi is released under GPL license


