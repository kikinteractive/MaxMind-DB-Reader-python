.. :changelog:

History
-------

1.0.0 (2014-09-22)
++++++++++++++++++

* First production release.
* Two potential C extension issues discovered by Coverity were fixed:
  - There was a small resource leak that occurred when the system ran out of
    memory.
  - There was a theoretical null pointer issue that would occur only if
    libmaxminddb returned invalid data.

0.3.3 (2014-04-09)
++++++++++++++++++

* Corrected initialization of objects in C extension and made the objects
  behave more similarly to their pure Python counterparts.

0.3.2 (2014-03-28)
++++++++++++++++++

* Switched to Apache 2.0 license.
* We now open the database file in read-only mode.
* Minor code clean-up.

0.3.1 (2014-02-11)
++++++++++++++++++

* Fixed packaging problem that caused ``import`` to fail.

0.3.0 (2014-02-11)
++++++++++++++++++

* This release includes a pure Python implementation of the database reader.
  If ``libmaxminddb`` is not available or there are compilation issues, the
  module will fall-back to the pure Python implementation.
* Minor changes were made to the exceptions of the C extension make them
  consistent with the pure Python implementation.

0.2.1 (2013-12-18)
++++++++++++++++++

* Removed -Werror compiler flag as it was causing problems for some OS X
  users.

0.2.0 (2013-10-15)
++++++++++++++++++

* Refactored code and fixed a memory leak when throwing an exception.

0.1.1 (2013-10-03)
++++++++++++++++++

* Added MANIFEST.in

0.1.0 (2013-10-02)
++++++++++++++++++

* Initial release
