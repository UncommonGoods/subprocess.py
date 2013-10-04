subprocess.py
=============

Basically, Python's subprocess module was escaping arguments with double quotes, and this wasn't really "doing it" for me.

Now `Popen` takes a `singlequote` boolean argument that uses single quotes instead of double quotes, if True.

<b>The End.</b>
