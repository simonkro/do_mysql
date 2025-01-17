## 0.10.7 2011-10-13

* Ruby 1.9.3 compatibility

## 0.10.6 2011-05-22

Bugfixes
* Fix an issue on some platforms when multiple DO drivers are loaded

## 0.10.5 2011-05-03

No changes

## 0.10.4 2011-04-28

New features
* Add save point to transactions (all)
* JRuby 1.9 mode support (encodings etc.)

Bugfixes
* Fix bug when using nested transactions in concurrent scenarios (all)
* Use column aliases instead of names (jruby)
* DST calculation fixes (all)
* Attempt to add better support for ancient MySQL versions (do\_mysql)

Other
* Refactor to DRY up the adapters (all)
* Many style fixes
* Switch back to RSpec

## 0.10.3 2011-01-30
* Reworked transactions
* Fix a DST bug that could cause datetimes in the wrong timezone

## 0.10.2 2010-05-19
* Make sure Text is returned in the proper encoding
* Make Encoding.default_internal aware
* Fix insert_id if no incrementing key is used
* Rework logging for making callbacks possible
* Remove handling Object types directly

## 0.10.1 2010-01-08

* Support for Ruby 1.8 and 1.9 on Windows.
* Switch to Jeweler for Gem building tasks (this change may be temporary).
* Switch to using Bacon for running specs: This should make specs friendlier to
  new Ruby implementations that are not yet 100% MRI-compatible, and in turn,
  pave the road for our own IronRuby and MacRuby support.
* Switch to the newly added rake-compiler `JavaExtensionTask` for compiling
  JRuby extensions, instead of our (broken) home-grown solution.

## 0.10.0 2009-09-15
* Improvements
  * JRuby Support (using *do_jdbc*)

## 0.9.12 2009-05-17
* Improvements
  * Windows support

## 0.9.11 2009-01-19
* Improvements
  * Ruby 1.9 support
* Fixes
  * Reconnecting now works properly

## 0.9.9 2008-11-27
* Improvements
  * Added initial support for Ruby 1.9 [John Harrison]
