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

使用脚本安装和升级pip
----------------------

要安装或升级pip，需要下载 `get-pip.py
<https://raw.github.com/pypa/pip/master/contrib/get-pip.py>`_. [1]_

然后运行以下命令 (需要管理员权限)::

 $ python get-pip.py

如果 `setuptools`_ (或 `distribute`_) 未安装, ``get-pip.py`` 会
自动为你安装 `setuptools`_ . [2]_

如果需要升级 `setuptools`_ (或 `distribute`_), 运行 ``pip install -U setuptools`` [3]_


使用软件管理器安装
----------------------

在Linux系统中，pip通常可以在系统的软件管理器中安装，不过通过此方法安装的
一般不会是最新版本的pip.

Debian 和 Ubuntu::

   $ sudo apt-get install python-pip

Fedora::

   $ sudo yum install python-pip


.. [1] "Secure" in this context means using a modern browser or a
       tool like `curl` that verifies SSL certificates when downloading from
       https URLs.

.. [2] 从 pip v1.5.1开始, 使用 ``get-pip.py`` 安装pip不一定需要先安装setuptools.

.. [3] Although using ``pip install --upgrade setuptools`` to upgrade from
       distribute to setuptools works in isolation, it's possible to get
       "ImportError: No module named setuptools" when using pip<1.4 to upgrade a
       package that depends on setuptools or distribute. See :doc:`here for
       details <distribute_setuptools>`.

.. _setuptools: https://pypi.python.org/pypi/setuptools
.. _distribute: https://pypi.python.org/pypi/distribute
