util
====

ExpressionEngine plugin which allows to call few string processing php functions from your template. Has few other useful methods too


func
Execute any php function from template, You can pass function argument/constant too
Example:
{exp:util:func function="htmlentities" params="ENT_QUOTES|'UTF-8'"}A 'quote' is &lt;b&rt;bold&lt;/b&rt;{/exp:util:func}
{exp:util:func function="strip_tags" params="'&lt;p&rt;&lt;a&rt;'"}&lt;p&rt;Test paragraph.&lt;/p&rt;&lt;!-- Comment --&rt; &lt;a href="#fragment"&rt;Other text&lt;/a&rt;{/exp:util:func}
{exp:util:func function="strlen" data="Get string length"}

escape
Convert special characters to HTML entities
Example: {exp:util:escape data="&lt;a href='test'&rt;Test&lt;/a&rt;"}


join
Join a string by a specific glue
Example: {exp:util:join data="1,2,3,4" glue="|"}

first
Get first character of a string
Example:
{exp:util:first data="1,2,3,4"}&lt;br /&rt;
{exp:util:first data="1234"}

last
Get last character of a string
Example: {exp:util:last data="1,2,3,4"}
{exp:util:last data="1234"}
