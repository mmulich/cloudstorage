============
Contributing
============

Contributions are welcome, and they are greatly appreciated! Every
little bit helps, and credit will always be given.

Bug reports
===========

When `reporting a bug <https://github.com/scottwernervt/cloudstorage/issues>`_ please include:

    * Your operating system name and version.
    * Any details about your local setup that might be helpful in troubleshooting.
    * Detailed steps to reproduce the bug.

Documentation improvements
==========================

``cloudstorage`` could always use more documentation, whether as part of the
official ``cloudstorage`` docs, in docstrings, or even on the web in blog posts,
articles, and such.

Feature requests and feedback
=============================

The best way to send feedback is to file an issue at https://github.com/scottwernervt/cloudstorage/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions are welcome :)

Development
===========

To set up `cloudstorage` for local development:

1. `Fork cloudstorage on GitHub <https://github.com/scottwernervt/cloudstorage/fork>`_.

2. Clone your fork locally

::

    $ git clone git@github.com:your_name_here/cloudstorage.git

3. Install development requirements. It is **highly recommended** that you use a ``virtualenv``. Use the following command to install an editable version of marshmallow along with its development requirements.

::

    # After activating your virtualenv
    $ pip install -e '.[dev]'

4. Install the ``pre-commit`` hooks, which will format and lint your git staged files.

::

    # The pre-commit CLI was installed above
    $ pre-commit install --allow-missing-config

5. Create a branch for local development

::

    $ git checkout -b name-of-your-bugfix-or-feature

6. When you're done making changes, run all the checks, and doc builder with `tox <http://tox.readthedocs.io/en/latest/install.html>`_ one command

::

    $ tox

7. Commit your changes and push your branch to GitHub

::

    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature

8. Submit a pull request through the GitHub website.

Pull Request Guidelines
-----------------------

If you need some code review or feedback while you're developing the code just make the pull request.

For merging, you should:

1. Include passing tests (run ``tox``) [1]_.
2. Update documentation when there's new API, functionality etc.
3. Add a note to ``CHANGELOG.rst`` about the changes.

.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
       `run the tests <https://travis-ci.org/scottwernervt/cloudstorage/pull_requests>`_ for each change you add in the pull request.

       It will be slower though ...
