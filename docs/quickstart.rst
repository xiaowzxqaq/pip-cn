快速指南
==========

首先, :doc:`安装pip <installing>`.

从 `PyPI`_ 安装:

::

  $ pip install SomePackage
    [...]
    Successfully installed SomePackage

查看什么包被安装:

::

  $ pip show --files SomePackage
    Name: SomePackage
    Version: 1.0
    Location: /my/env/lib/pythonx.x/site-packages
    Files:
     ../somepackage/__init__.py
     [...]

查看什么包有更新:

::

  $ pip list --outdated
    SomePackage (Current: 1.0 Latest: 2.0)

更新新的模块包:

::

  $ pip install --upgrade SomePackage
    [...]
    Found existing installation: SomePackage 1.0
    Uninstalling SomePackage:
      Successfully uninstalled SomePackage
    Running setup.py install for SomePackage
    Successfully installed SomePackage

卸载已有包:

::

  $ pip uninstall SomePackage
    Uninstalling SomePackage:
      /my/env/lib/pythonx.x/site-packages/somepackage
    Proceed (y/n)? y
    Successfully uninstalled SomePackage


.. _PyPI: http://pypi.python.org/pypi/
