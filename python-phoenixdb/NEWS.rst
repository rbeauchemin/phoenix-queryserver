Changelog
=========

Version 1.1.0
-------------

- Implemented get_primary_keys() and get_index_info() methods in meta object (PHOENIX-6410)
- Fixed broken SqlAlchemy get_pk_constraint() method to use meta.get_primary_keys() (PHOENIX-6410)
- Implemented SqlAlchemy get_indexes() method to expose meta.get_index_info() (PHOENIX-6410)
- Fixed empty array column handling in result set (PHOENIX-6484)

Version 1.0.1
-------------

- Use HTTP sessions to enable sticky load balancers (PHOENIX-6459)
- Revert default GSSAPI OID to SPNEGO to improve compatibility (PHOENIX-6414)

Version 1.0.0
-------------

- Replaced bundled requests_kerberos with request_gssapi library
- Use default SPNEGO Auth settings from request_gssapi
- Refactored authentication code
- Added support for specifying server certificate
- Added support for BASIC and DIGEST authentication
- Fixed HTTP error parsing
- Added transaction support
- Added list support
- Rewritten type handling
- Refactored test suite
- Removed shell example, as it was python2 only
- Updated documentation
- Added SQLAlchemy dialect
- Implemented Avatica Metadata API
- Misc fixes
- Licensing cleanup

Version 0.7
-----------

- Added DictCursor for easier access to columns by their names.
- Support for Phoenix versions from 4.8 to 4.11.

Version 0.6
-----------

- Fixed result fetching when using a query with parameters.
- Support for Phoenix 4.9.

Version 0.5
-----------

- Added support for Python 3.
- Switched from the JSON serialization to Protocol Buffers, improved compatibility with Phoenix 4.8.
- Phoenix 4.6 and older are no longer supported.

Version 0.4
-----------

- Fixes for the final version of Phoenix 4.7.

Version 0.3
-----------

- Compatible with Phoenix 4.7.

Version 0.2
-----------

- Added (configurable) retry on connection errors.
- Added Vagrantfile for easier testing.
- Compatible with Phoenix 4.6.

Version 0.1
-----------

- Initial release.
- Compatible with Phoenix 4.4.
