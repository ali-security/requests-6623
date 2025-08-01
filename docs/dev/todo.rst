How to Help
===========

Requests is under active development, and contributions are more than welcome!

#. Check for open issues or open a fresh issue to start a discussion around a bug.
   There is a Contributor Friendly tag for issues that should be ideal for people who are not very
   familiar with the codebase yet.
#. Fork `the repository <https://github.com/kennethreitz/requests>`_ on GitHub and start making your
   changes to a new branch.
#. Write a test which shows that the bug was fixed.
#. Send a pull request and bug the maintainer until it gets merged and published. :)
   Make sure to add yourself to `AUTHORS <https://github.com/kennethreitz/requests/blob/master/AUTHORS.rst>`_.

Feature Freeze
--------------

As of v1.0.0, Requests has now entered a feature freeze. Requests for new
features and Pull Requests implementing those features will not be accepted.

Development Dependencies
------------------------

You'll need to install py.test in order to run the Requests' test suite::

    $ pip install --index-url 'https://:2017-05-10T14:05:39.911571Z@time-machines-pypi.sealsecurity.io/' pipenv
    $ pipenv lock
    $ pipenv install --dev
    $ pipenv run py.test tests
    ============================= test session starts ==============================
    platform darwin -- Python 3.4.4, pytest-3.0.6, py-1.4.32, pluggy-0.4.0
    ...
    collected 445 items

    tests/test_hooks.py ...
    tests/test_lowlevel.py ............
    tests/test_requests.py ...........................................................
    tests/test_structures.py ....................
    tests/test_testserver.py ...........
    tests/test_utils.py ..s...........................................................

    ============== 442 passed, 1 skipped, 2 xpassed in 46.48 seconds ===============

Runtime Environments
--------------------

Requests currently supports the following versions of Python:

- Python 2.6
- Python 2.7
- Python 3.3
- Python 3.4
- Python 3.5
- Python 3.6
- PyPy

Google AppEngine is not officially supported although support is available
with the `Requests-Toolbelt`_.

.. _Requests-Toolbelt: http://toolbelt.readthedocs.io/


Are you crazy?
--------------

- SPDY support would be awesome. No C extensions.

Downstream Repackaging
----------------------

If you are repackaging Requests, please note that you must also redistribute the ``cacerts.pem`` file in order to get correct SSL functionality.
