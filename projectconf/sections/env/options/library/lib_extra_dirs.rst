..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _projectconf_lib_extra_dirs:

``lib_extra_dirs``
------------------

.. seealso::
    Please make sure to read :ref:`ldf` guide first.

Type: ``DirPath`` | Multiple: ``Yes``

A list with extra directories/storages where :ref:`ldf` will
look for dependencies.

This option can also be set by global environment variable
:envvar:`PLATFORMIO_LIB_EXTRA_DIRS`.

.. warning::
  This is a not direct path to a library with source code. It should be a path
  to storage that contains libraries grouped by folders. For example,
  ``D:\PlatformIO\extra\libraries`` but not ``D:\PlatformIO\extra\libraries\FooLibrary``.

Example:

.. code-block:: ini

    [env:myenv]
    lib_extra_dirs =
        /common/libraries
        /iot/libraries