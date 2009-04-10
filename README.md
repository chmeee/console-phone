# Console phone

## What's this

This tries to document an idea I had about developing a console phone, that is,
a text-based phone without all the GUI-phones blues around. 

## Motivation

I like the command-line, I use vim, sup, vimperator, wmii, etc. and I like the
way it feels. So I thought, maybe a console phone is also easy and nice to use.
I haven't found any phones like that (yet) and neither any specification.

So this document tries to be an initial draft of what I mean and see if someone
finds it interesting.

## Specification (sort of)

### Interface

The phone will have a 'gnu screen' like interface where you can switch between
different screens with different uses.

The main user screen is a command-line interface using 'gnu readline' with a
prompt (something short line '>' or '$' or '#'). This is the interface to place
calls and run commands. All commands and 'subjects' will have auto-completion.

Commands allowed:

* call
* add (contact)
* edit (contact)
* mail
* sms
* chat
* tweet
* web
* contacts
* history
* config

There can be an bottom 'status line' where operator, time, battery and signal
are shown.

An upcomming call would switch the screen to the command line and you'll get
something like:

    > INCOMMING CALL FROM chmeee
    answer? [Y/n]

### Keyboard

I'm not sure about this. If there should be a text-based onscreen keyboard or a
physical one. In any case, even if it's a graphical keyboard (in the case the
console-phone app is running inside a GUI phone), the keyboard must be good
enough, otherwise, user experience will be crap.

### Apps

Console apps are already there. Curses apps would be great.

* sup for mail
* links for web
* finch for chat
* ruby twitter gem for tweet

### Games

Any text-based game:

* Of course it will have the 'text-based' nethack, best game ever.
* Another good addtion would be gnu-go.
* Adventure, and other conversational games.

## Implementation

I wish the console phone got implemented in ruby. That way you can always drop
to 'irb' from the command-line interface and do some ruby magic in your phone.

If I get to finish (one of these days) my degree project I'll implement one
basic functionality just for fun :). 

Feel free to fork and update this readme or contribute with sample code.
