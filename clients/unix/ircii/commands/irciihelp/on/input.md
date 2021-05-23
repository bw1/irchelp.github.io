---
title: 'ircii help: input'
author: Michael Sandrof, Troy Rollo, Matthew R. Green
datecreated: 3 August 2020
layout: default
license: ircii
summary: >
  ircii version: 20190117
  create with help2md.pl
---
```
Usage: ON [#|+|-|^|&|@]INPUT [-|^]<parameters> [action]
  This is activated whenever you send a line of input to either
  a channel or a query user.  This means that if you type in a
  message and hit return, ON INPUT can be activated.
  ON INPUT can catch and process any input line.

Note: The fact that you can capture any line and suppress further
  normal processing means you can completely disable the client
  by accident or on purpose.  Don't use this function if you don't
  know exactly what you are trying to do.
  Parameters are:
	$0	Text of line
  If you use ^ to suppress the processing of the line, you can 
  do your own pre-processing and send the line back to the client 
  with a call to SENDLINE.
  Note $[1]0 is the first character of the first word of the line.
  Also, the $T var can show you who or what you're talking to at
  any given moment.

```
See Also:
  [SET INPUT_PROTECTION](../set/input_protection.html)
  [ALIAS special](../alias/special.html)

[index](index.html)
[up](..)

<small> ircii 20190117 </small>