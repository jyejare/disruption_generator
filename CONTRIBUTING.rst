.. highlight:: shell

============
Contributing
============

Contributions are welcome, and they are greatly appreciated! Every little bit
helps, and credit will always be given.

You can contribute in many ways:

Types of Contributions
----------------------

Report Bugs
~~~~~~~~~~~

Report bugs at https://github.com/grafuls/disruption_generator/issues.

If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

Fix Bugs
~~~~~~~~

Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
wanted" is open to whoever wants to implement it.

Implement Features
~~~~~~~~~~~~~~~~~~

Look through the GitHub issues for features. Anything tagged with "enhancement"
and "help wanted" is open to whoever wants to implement it.

Write Documentation
~~~~~~~~~~~~~~~~~~~

Disruption Generator could always use more documentation, whether as part of the
official Disruption Generator docs, in docstrings, or even on the web in blog posts,
articles, and such.

Submit Feedback
~~~~~~~~~~~~~~~

The best way to send feedback is to file an issue at https://github.com/grafuls/disruption_generator/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions
  are welcome :)

.. _getting-started-label:

Get Started!
------------

Ready to contribute? Here's how to set up `disruption_generator` for local development.

1. Fork the `disruption_generator` repo on GitHub.
2. Clone your fork locally::

    $ git clone git@github.com:your_name_here/disruption_generator.git

3. Install your local copy into a pipenv virtualenv. Assuming you have pipenv installed, this is how you set up your fork for local development::

    $ cd disruption_generator/
    $ pipenv install --dev
    $ pipenv shell
    $ python setup.py install

4. Create a branch for local development::

    $ git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

5. When you're done making changes, check that your changes pass flake8 and the
   tests, including testing other Python versions with tox::

    $ flake8 disruption_generator tests
    $ python setup.py test or py.test
    $ tox

   To get flake8 and tox, just pip install them into your virtualenv.

6. Commit your changes and push your branch to GitHub::

    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature

7. Submit a pull request through the GitHub website.

Pull Request Guidelines
-----------------------

Before you submit a pull request, check that it meets these guidelines:

1. The pull request should include tests.
2. If the pull request adds functionality, the docs should be updated. Put
   your new functionality into a function with a docstring, and add the
   feature to the list in README.rst.
3. The pull request should work for Python 3.5 and 3.6. Check
   https://travis-ci.org/grafuls/disruption_generator/pull_requests
   and make sure that the tests pass for all supported Python versions.
4. Finally, before you submit your pull request, make sure its name is prefixed
   either with:

   * [WIP] tag if you still intend to work on it or
   * [RFR] tag if it is ready to be reviewed by other contributors.

   .. warning:: Pull requests that are not prefixed with [RFR] will be ignored!

Code Style
----------

We of course stick to PEP8 recommendations. Max line length is 120 characters.

Tips
----

To run a subset of tests::

   $ py.test tests.test_disruption_generator

To build documentation locally::

   $ make docs

You can also let the docs be built dynamically while working on them.
You can see sphinx output in console and you can see your changes straight away in browser (that is after you hit
refresh button). You can achieve this by::

   $ make servedocs
