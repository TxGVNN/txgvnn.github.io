This package implements a generic interface for toggling switches
and setting options and then invoking an Emacs command which does
something with these arguments.  The prototypical use is for the
command to call an external process, passing on the arguments as
command line arguments.  But this is only one of many possible
uses (though the one this library is optimized for).

With the Emacs concept of "prefix arguments" in mind this could be
described as "infix arguments with feedback in a buffer".

Commands that set the prefix argument for the subsequent command do
not limit what that next command could be.  But entering a command
console popup does limit the selection to the commands defined for
that popup, and so we use the term "infix" instead of "prefix".
