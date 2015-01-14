# Angular-BBcode-Filter
An Angular filter for parsing bbcode client side

This is a work in progress. I will be adding new bbcode as I need them. I found [node-bbcode][],
but wanted something client side instead.


I've made this to be easily edited or expanded.

The main function runs string.replace() using regular expressions to find the bbcode. Currently the regex will find:
* p1  =   opening tag
* p2  =   opening tag value
* p3  =   opt tag 1 length 1-3
* p4  =   opt tag 1 value
* p5  =   opt tag 2 length 1-16
* p6  =   opt tag 2 value
* p7  =   text between opening & closing tags
* p8  =   closing tag

To edit/add tag parsing just change what happens in the switch statement. If you are adding custom tags make sure to add the tags value to valid_tags_re regular expression.

TODO: Still need to add most of the tags. This is a part of a larger project so I will be adding as I go.

[node-bbcode]: https://github.com/ncb000gt/node-bbcode
