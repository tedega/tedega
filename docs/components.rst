Komponenten
===========
Wie in im Abschnitt :ref:`architecture` beschrieben, besteht eine Microservice aus
verschiednen Komponenten. In diesem Abschnitt sollen diese Komponenten näher
in ihrer Funktion und Aufgaben beschrieben werden. Dabei werden insbesondere
die Schnittstellen beschrieben, die für die Implementation einer Domain
genutzt werden können bzw. müssen.

.. index::
   pair: Komponenten; Core
.. _core:

Core
----

.. index::
   pair: Komponenten; Service
.. _service:

Service
-------

.. index::
   pair: Komponenten; Storage

.. autofunction:: tedega_service.registry.config_service_endpoint
.. autofunction:: tedega_service.service.start_service

.. _storage:

Storage
-------

.. index::
   pair: Komponenten; CLI

.. autofunction:: tedega_storage.storage.init_storage
.. autofunction:: tedega_storage.storage.get_storage
.. autofunction:: tedega_storage.storage.scoped_session
.. autoclass:: tedega_storage.storage.Storage
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
