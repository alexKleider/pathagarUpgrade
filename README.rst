==============
PathagarUpdate
==============

An attempt to upgrade pathagar (as found at `github
<https://github.com/PathagarBooks/pathagar>`) to use the
current (v1.10.5) version of Django (as well as current 
versions of other dependencies. See require.txt.)

For now there isn't much to add to what appears in the first commit
message which follows.

------------
First commit
------------

On my development machine (my laptop) a top level directory
``/Pj`` has been created ('Pj' stands for Project.)
Under this directory I've placed ``virtualenv`` files and ``Django``
project directory files.
The project directory files include ``pathagar`` which is a clone of
https://github.com/PathagarBooks/pathagar
and ``p2`` which is my fledgling attempt to upgrade ``pathagar`` to
the latest version of ``Django``.
The two ``virtualenv`` files found under ``/Pj`` are
``oldVenv``: the environment created from
``pathagar/requirements.pip``,
and
``venv``: an environment created from ``p2/require.txt``, which was
simply a copy of ``pathagar/requirements.pip`` with all the '=='
changed to '>='.  I believe (but am not absolutely certain) the
command used was ``pip install --upgrade -r require.txt``.

Then it was simply a matter of creating a ``Django`` project: ``p2``
which set up the directory structure found there.
My work so far has been to edit the ``p2/p2/settings.py`` file to
include all the content of ``pathagar/settings.py`` in a form that is
acceptable to the latest version of ``Django``.

That's as far as I've gotten so far.
