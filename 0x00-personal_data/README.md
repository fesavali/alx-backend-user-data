This module defines functions and classes which implement a flexible event logging system for applications and libraries.

The key benefit of having the logging API provided by a standard library module is that all Python modules can participate in logging, so your application log can include your own messages integrated with messages from third-party modules.

The simplest example:

>>> import logging
>>> logging.warning('Watch out!')
WARNING:root:Watch out!
The module provides a lot of functionality and flexibility. If you are unfamiliar with logging, the best way to get to grips with it is to view the tutorials (see the links above and on the right).

The basic classes defined by the module, together with their functions, are listed below.

Loggers expose the interface that application code directly uses.

Handlers send the log records (created by loggers) to the appropriate destination.

Filters provide a finer grained facility for determining which log records to output.

Formatters specify the layout of log records in the final output.