# Realtime WYSIWYG Editor Binding

This binding makes use of the [chainpad][chainpad] realtime editor engine and binds
to the [XWiki WYSIWYG][wysiwyg] editor. It is currently a work-in-progress but to try it out,
install use the [XWiki Realtime Backend][rtbackend] from the Extension Manager and build the .xar file
as follows:

    # first make sure you have an up-to-date version of xwiki-tools
    git clone git://github.com/xwiki-contrib/node-xwikimodel.git
    cd node-xwikimodel
    npm install -g

    # then run the builder
    ./do

    # and import the resulting XAR file.

Alternatively you can build and import in one operation using:

    ./do --post Admin:admin@mywikidomain.name:8080/xwiki

Or generate a Maven compatible build using:

    ./do --mvn

Issues: http://jira.xwiki.org/browse/RTWYSIWYG


[chainpad]: https://github.com/xwiki-contrib/chainpad
[wysiwyg]: http://extensions.xwiki.org/xwiki/bin/view/Extension/WYSIWYG+Editor+Module
[rtbackend]: http://extensions.xwiki.org/xwiki/bin/view/Extension/RtBackend
