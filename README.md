util
====

ExpressionEngine plugin which allows to call few string processing php functions from your template. Has few other useful methods too

```
<strong>func</strong>
Execute any php function from template, You can pass function argument/constant too
Example:
{exp:util:func function="htmlentities" params="ENT_QUOTES|'UTF-8'"}A 'quote' is <b>bold</b>{/exp:util:func}
{exp:util:func function="strip_tags" params="'<p><a>'"}<p>Test paragraph.</p><!-- Comment --> <a href="#fragment">Other text</a>{/exp:util:func}
{exp:util:func function="strlen" data="Get string length"}

<strong>escape</strong>
Convert special characters to HTML entities
Example: {exp:util:escape data="<a href='test'>Test</a>"}


<strong>join</strong>
Join a string by a specific glue
Example: {exp:util:join data="1,2,3,4" glue="|"}

<strong>first</strong>
Get first character of a string
Example:
{exp:util:first data="1,2,3,4"}<br />
{exp:util:first data="1234"}

<strong>last</strong>
Get last character of a string
Example: {exp:util:last data="1,2,3,4"}
{exp:util:last data="1234"}
```