To be able to use Omegle in all circumstances and not be 'stuck' in a browser!

In the first version, some code was taken from the Omegle Bot found at
http://pastebin.com/m67ea2891

I must thank "thedotmaster" for his awesome reverse-engineering, found at http://forums.hackthissite.org/viewtopic.php?f=37&t=3783

Let me explain it:

When you first want to engage in a conversation, you need the stranger ID. (/start)
After it is acquired, you can speak to it by sending the Message and the ID, as a string to the send page (this is all AJAX).
All the events (waiting, connected, typing, gotMessage+data, strangerDisconnected) can be listened at the events page.