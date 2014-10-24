Path: Path for Pretty People
============================

path provide highly **readable** API for OS path manipulation and accessing filesystem. All operations are
available at module level as functions.

    >>> import path
    >>> path.cwd() # return current working directory.
    >>> path.chd() # change current working directory.
    ...
    
Operations are available as `Path` object methods too.

    >>> p = path.Path('c:\\hello\world.py')
    >>> p.name
    'world'
    >>> p.ext
    '.py'
    >>> p.ispath(path.EXIST) # check path or file existence.
    >>> p.isempty() # whether the file or dir is empty.
    ...
    
Individual classes for readability.

    >>> comp = path.Components('c:\\hello\world.py')
    >>> comp.name
    'world'
    >>> comp.ext
    '.py'
    
Unlike other packages, path also work on **URL** too. Which ease web-scrapper coding.

    >>> p = path.HttpPath('https://github.com/docopt/docopt')
    >>> p.path
    '/docopt/docopt'
    >>> p.create() # will create dir or file according to args.
    ...

Features
--------

- Work both on path and URL
- Highly readable API
- Provide constants
- Operations are available as functions and methods
- Individual classes for everything

Installation
------------

    $ pip install https://github.com/mahanmarwat/path

Documentation
-------------

Under development.

Contribute
----------

Give us a star.