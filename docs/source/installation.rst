.. include:: links.rst

-------------
Installation
-------------
How to install fcdproc package:

* within a `Manually Prepared Environment (Python 3.7+)`_, also known as
  *bare-metal installation*;

Once you have your *bare-metal* environment set-up (first option above),
the next step is executing the ``fcdproc`` command-line.
The ``fcdproc`` command-line options are documented in the :ref:`usage`
section.

The ``fcdproc`` command-line adheres to the `BIDS-Apps recommendations
for the user interface <usage.html#execution-and-the-bids-format>`__.
Therefore, the command-line has the following structure:
::

  $ fcdproc <input_bids_path> <derivatives_path> <analysis_mode> <named_options>


Manually Prepared Environment (Python 3.7+)
===========================================
Make sure all of *fcdproc*'s `External Dependencies`_ are installed.
These tools must be installed and their binaries available in the
system's ``$PATH``.
As an additional installation setting, FreeSurfer requires a license file (see :ref:`fs_license`).


On a functional Python 3.7 (or above) environment with ``pip`` installed,
*fcdproc* can be installed using the habitual command ::

    $ python -m pip install fcdproc

Check your installation with the ``--version`` argument ::

    $ fcdproc --version


External Dependencies
---------------------
*fcdproc* is written using Python 3.7 (or above), and is based on
nipype_.


*fcdproc* requires some other neuroimaging software tools that are
not handled by the Python's packaging system (Pypi) used to deploy
the ``fcdproc`` package:

- AFNI_ (version Debian-16.2.07)
- FreeSurfer_ (version 6.0.1)
- `bids-validator <https://github.com/bids-standard/bids-validator>`_ (version 1.4.0)