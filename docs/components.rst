Komponenten
===========
Wie in im Abschnitt :ref:`architecture` beschrieben, besteht eine Microservice aus
verschiednen Komponenten. In diesem Abschnitt sollen diese Komponenten näher
in ihrer Funktion und Aufgaben beschrieben werden. Dabei werden insbesondere
die Schnittstellen beschrieben, die für die Implementation einer Domain
genutzt werden können bzw. müssen.

.. index::
   pair: Komponenten; Core
.. _share:

Share
-----

Logging
^^^^^^^

.. autofunction:: tedega_share.logger.get_logger
.. autoclass:: tedega_share.logger.Logger
   :members: debug, info, warning, error

.. index::
   pair: Komponenten; View
.. _view:

View
----

.. index::
   pair: Komponenten; Storage

.. autofunction:: tedega_view.registry.config_view_endpoint
.. autofunction:: tedega_view.server.start_server

.. _storage:

Storage
-------

.. index::
   pair: Komponenten; CLI

.. autofunction:: tedega_storage.rdbms.init_storage
.. autofunction:: tedega_storage.rdbms.get_storage
.. autofunction:: tedega_storage.rdbms.scoped_session
.. autoclass:: tedega_storage.rdbms.storage.Storage
   :members:

.. Logging
.. -------
..
.. .. index::
..    pair: Komponenten; Logging
..    pair: Fluentd; Logging
..
.. MessageQueue
.. ------------
..
.. .. index::
..    pair: Komponenten; MessageQueue
..    pair: RabbitMQ; MessageQueue

.. .. index::
..    pair: Komponenten; Domain
.. .. _domain:
..
.. Domain
.. ------
..
.. Konfiguration
.. ^^^^^^^^^^^^^
..
.. Server
.. """"""
.. Datenbank
.. """""""""
.. * **TEDEGA_STORAGE_URI** Vorgabe ist eine flüchtige sqlite DB im
..   Speicher.
