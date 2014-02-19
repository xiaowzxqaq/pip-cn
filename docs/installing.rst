.. _`Installation`:

安装pip
============

Python和系统版本支持列表
-------------------

pip可以在以下版本的CPython下运行：2.6, 2.7, 3.1, 3.2, 3.3, 3.4 和 pypy.

pip可以在Unix/Linux, OS X 和 Windows系统中运行.

.. note::

  Python 2.5在 v1.3.1版本后支持, Python 2.4在v1.1版本后支持.


.. _`get-pip`:

安装和升级pip
----------------------

要安装或升级pip，需要下载 `get-pip.py
<https://raw.github.com/pypa/pip/master/contrib/get-pip.py>`_. [1]_

然后运行以下命令 (需要管理员权限)::

 $ python get-pip.py

如果 `setuptools`_ (或 `distribute`_) 未安装, ``get-pip.py`` 会
自动为你安装 `setuptools`_ . [2]_

如果需要升级 `setuptools`_ (或 `distribute`_), 运行 ``pip install -U setuptools`` [3]_


使用包管理器
----------------------

On Linux, pip will generally be available for the system install of python using
the system package manager, although often the latest version will be
unavailable.

On Debian and Ubuntu::

   $ sudo apt-get install python-pip

On Fedora::

   $ sudo yum install python-pip


.. [1] "Secure" in this context means using a modern browser or a
       tool like `curl` that verifies SSL certificates when downloading from
       https URLs.

.. [2] Beginning with pip v1.5.1, ``get-pip.py`` stopped requiring setuptools to
       be installed first.

.. [3] Although using ``pip install --upgrade setuptools`` to upgrade from
       distribute to setuptools works in isolation, it's possible to get
       "ImportError: No module named setuptools" when using pip<1.4 to upgrade a
       package that depends on setuptools or distribute. See :doc:`here for
       details <distribute_setuptools>`.

.. _setuptools: https://pypi.python.org/pypi/setuptools
.. _distribute: https://pypi.python.org/pypi/distribute
