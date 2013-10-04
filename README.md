subprocess.py
=============

UncommonGoods fork of the python "subprocess" library.

We were experiencing some problems with the way the library was escaping arguments for Windows CLI, so we modified the lib2cmdline method.

To enclose arguments with single quotes rather than double quotes, you can pass the `singlequote` parameter. For example:

<pre>
output = subprocess.check_output(\
    ['powershell', r'.\my_script.ps1', 'An argument - that should & be single-quoted'],\
    singlequote=True)
</pre>

Copied from BitBucket: https://bitbucket.org/pypy/pypy/src/9d88b4875d6e/lib-python/2.7/subprocess.py
