###############
Contributing 🎉
###############

**Thanks for your interest!** All contributions are welcome. We feel this library will grow stronger from user contributions, so thank you for your time.

To maintain consistency across the code base (and minimize the introduction of bugs), we follow several guidelines. Every effort has been made to automate this for you using several tools so you can focus on adding features rather than fixing semicolons.

This page is meant to show you how to use these tools and what rules to follow when contributing code. Please read the following sections very carefully.

-----

Guidelines
==========

Being Respectful
----------------

First and foremost, all contributors shall demonstrate empathy and kindness towards each other. This project respects all skill levels and aims to foster an environment where people want to contribute. Please do not talk down or belittle others or their work. For more info, please read the `Code of Conduct`_.

Branching and Versioning Strategy
---------------------------------

``pyvista-view`` adopts a `0-ver`_ / `PEP 440`_-ish style versioning strategy with a `GitHub Flow`_-ish style branching strategy. The rationale for this choice is best summarized as follows:

    *"version numbers are just a mapping of a sequence of digits to our branching strategy in source control"*

    -- `Brett Cannon`_

Testing
-------

``tox`` is used to test code. To use ``uv`` virtual environments with ``tox``, install ``tox-uv`` as a tool:

.. code-block:: bash

   uv tool install tox --with tox-uv --force-reinstall


To run tests, execute the following:

.. code-block:: bash

   uvx tox

which is set to run

.. code-block:: bash

   coverage run -m pytest

for all Python versions this package supports.

Becoming a Maintainer
---------------------

If you feel you can triage problems and mentor junior developers, please consider becoming a maintainer! For more info, please `contact the author`_.

.. _`Code of Conduct`:
   code_of_conduct.rst
.. _`0-ver`:
   https://0ver.org/
.. _`PEP 440`:
   https://peps.python.org/pep-0440/#public-version-identifiers
.. _`GitHub Flow`:
   https://docs.github.com/en/get-started/quickstart/github-flow
.. _`Brett Cannon`:
   https://snarky.ca/why-i-dont-like-semver/
.. _`contact the author`:
   mailto:adam.grant.hendry@gmail.com
