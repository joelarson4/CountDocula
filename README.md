#Count Docula ᗑⓦᗑ

##I vant to make Markdown from your JavaScript documentation, AH AH AH!

This repo is a placeholder at the moment.  I would like to create a tool that would make it easy to turn JSDoc-like comments in JavaScript into GitHub friendly Markdown.  For example, a JavaScript file containing:

    /**
     *  Used to do some important thing that needs doing that works like xyz.
     *  @param {String} whatever - some string that has some purpose
     *  @param {Function} callback - a function that needs to be run
     *  @returns {Boolean} whether or not something happened
     */
     function something(whatever, callback) {
         ...

would produce nice markdown:

    ##`root.something(whatever,callback)`
    Used to do some important thing that needs doing that works like xyz.

    *Parameters*
      `whatever {String}` some string that has some purpose
      `callback {Function}` a function that needs to be run

    *Returns*
       `{Boolean}` whether or not something happened

For some more background on my train of thought, check out this StackOverflow question: http://stackoverflow.com/questions/15694267/how-to-easily-create-github-friendly-markdown-for-documented-javascript-function


##Goals

Primary goals:

+ Very easy to get started with
+ Compatible with all commonly used JSDoc tags
+ Module aware and capable (CommonJS and AMD)

Secondary goals:

+ Template driven output
+ Extensible
+ Grunt integration


##What's next

I need to dig into the existing JavaScript documentation tools and see if any can be bent into service of this cause.  I think that https://github.com/visionmedia/dox could be a good starting point.


