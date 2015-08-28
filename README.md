Troubleshoot!
=============

**WARNING!!  This is a joke!** It will not solve your Linux problems, but it is
pretty funny.  It says it runs commands, but it will only print them, for
entertainment purposes (see the disclaimer below).

In Windows, when something goes wrong, Microsoft gives its users some convenient
troubleshooting wizards that guide them through figuring out what's wrong.
Linux doesn't have that, and I think it's a shame.  Instead, we have to Google
our problem and keep trying solutions until we find the one that works.

Now, I present the end of an era for Linux users.  No longer will we have to
troubleshoot manually.  Instead, this program will automate your troubleshooting
tasks!  Simply run `./troubleshoot [describe your problem here]`, and it will
automatically search Google, find the first result with commands to run, and
execute all the code on that page.  For maximum effectiveness, you may need to
run `sudo ./troubleshoot [describe your problem here]`.

Installation
------------

Unfortunately, you have to have `requests` and `lxml` installed.  The nicest way
to get everything running is:

```bash
pyvenv venv
. venv/bin/activate
pip install -r requirements.txt
./troubleshoot ...
```

You could also just make sure you have your distribution's Python 3, Requests,
and LXML packages installed.  Whatever floats your boat.


Disclaimer
----------

This program would be, like, super mega awfully damaging if anyone actually ran
it.  So, before I put this on GitHub, I replaced the shell (`bash`) with `cat`,
so that instead of *running* the commands, it would just *print* what it would
have run.  If you had a virtual machine or a computer you didn't mind
potentially destroying, then you could go in and replace `cat` with `bash`.
However, I take no responsibility for the results of this!
