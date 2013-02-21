Similar to jslint_uncommited, but using JSHint instead of JSLint 
For JSLint: https://github.com/jschill/jslint_uncommited


jshint_uncommited
=================

JSHint uncommited javascript-files in a Git repository using Node.js

You can also use the pre-commit hook to lint your javascript-files on the fly when committing to your repository.


Requirements
------------

* Git
* Node
* JSHint
* ..and probably a Mac. I haven't tested it elsewhere.


Installation
------------

* Put the jshint_uncommited.js script somewhere in your git repository 
* Run "node jshint_uncommited.js"

Or if you want to use the pre-commit hook

* Put the jshint_uncommited.js script somewhere in your git repository 
* Put the pre-commit in your {project_root_dir}/.git/hooks directory
* Change the LINTSCRIPT variable in pre-commit to point to where you placed jshint_uncommited.js
* Make sure the pre-commit is executable, ie: "chmod +x pre-commit" or "chmod 755 pre-commit"


Credits
-------
* https://github.com/jrburke/dvcs_jslint
* https://github.com/wbecker/dvcs_hook-jslint-node
* http://www.madr.se/b/jslint-git-hook
* http://stackoverflow.com/questions/1837681/pre-commit-hook-for-jslint-in-mercurial-and-git
* https://gist.github.com/haschek/2595796