Wolves Among the Sheep
======================

Poisoning security tools that use obsolate crypto.

Please use this code to test if the security products in your reach use MD5 internally to fingerprint binaries and share your results by issuing a pull request updating the contents of `results/`!

Works-on-a-different-machine-than-mine version, feedback is welcome!

Dependencies
------------

* 32-bit Windows (virtual) machine (64-bit will probably break stuff - not tested)
* Visual Studio 2012 to compile the projects (Express will do)
* [Fastcoll](https://www.win.tue.nl/hashclash/) for collisions
* Optional: Cygwin+MinGW to compile Evilize

Usage
-----

Extract Fastcoll to the `fastcoll` directory. Name the executable `fastcoll.exe`

Use `shepherd.bat` to generate `wolf.exe` and `sheep.exe`:

```
> shepherd.bat YOURPASSWORD your_shellcode.raw
```

After this step you should have your two colliding binaries (`sheep.exe` and `wolf.exe` in the `evilize` directory).

For more information see the [tutorial of Peter Selinger](http://www.mathstat.dal.ca/~selinger/md5collision/), older revisions of this document or the source code...

References
----------

* [Poisonous MD5 - Wolves Among the Sheep](http://blog.silentsignal.eu/2015/05/29/poisonous-md5-wolves-among-the-sheep/)
* [Peter Selinger: MD5 Collision Demo](http://www.mathstat.dal.ca/~selinger/md5collision/)
* [How to make two binaries with same MD5](http://natmchugh.blogspot.co.uk/2015/05/how-to-make-two-binaries-with-same-md5.html)
* [Stop using MD5 now!](http://jumpespjump.blogspot.hu/2014/03/stop-using-md-5-now.html)

LICENSE
-------

Licenced under GNU/GPL if not otherwise stated.

