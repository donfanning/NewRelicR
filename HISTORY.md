## Version 0.3.0.1105

* Improve column labels with multi-column timeseries.

## Version 0.3.0.1104

* Fix edge case in nrdb_query when you are getting multiple summary values.

## Version 0.3.0.1003

* Add verbose option for nrdb_events
* Fix bug in nrdb_events where WHERE was ignored

## Version 0.3.0.1001

* Added verbose option for several calls to see the NRQL.

## Version 0.3.0.1000

* Removed `sample_events()` since it didn't do a good job of sampling.
* Renamed `get_top_transactions` to `nrdb_top_transactions` for consistency.
* Improved queries when the attributes were specified explicitly

## Version 0.2.0.1001

* Renamed `get_events` to `nrdb_events`.

## Version 0.2.0.1000

* Changed license from GPL2 to BSD
* Added `get_events` method to get contiguous chunks of events for a given criteria.

## Version 0.1.0.1011

* Fixed some parameters in the session calls in the nrdb API

## Version 0.1.0.1010

* Fixed problem calculating think time
* Switched to include BrowserInteractions now available with SPA monitoring

## Version 0.1.0.1009

* Updated the session functions in the NRDB API.  Added some new options.

## Version 0.1.0.1008

* Add support for loading PageActions in session data

## Version 0.1.0.1007

* Add end_time parameter to get top applications

## Version 0.1.0.1005

* Made verbose output an option; quiet by default
* Fix bug in managing query cache

## Version 0.1.0.1004

* Fix bug in `get_top_transactions()`

## Version 0.1.0.1003

* Bug fixes and warnings

## Version 0.1.0.1000

* Add `rpm_applications()` function
* Fixes and documentation
* Bumped feature version to 1.

## Version 0.0.0.9006

* Add batch fetching to the `rpm_query()` call.  This means it will respect the period
  parameter and simply fetch data in chunks to get the resolution you need.
* New method for nrdb, `sample_events()` which selects a requested number of events near a point in time
  which may not be contiguous (hence "sample").  

## Version 0.0.0.9003

* Support for multi column timeseries queries, like `select average(duration), count(*) from Transaction timeseries AUTO`

## Version 0.0.0.9002

* Removed dependency on plyr
* Removed `%>%` usage

## Version 0.0.0.9001

* Removed `newrelic_api` helper in favor of passing api keys directly to functions
* Fixed many bugs
* Added some examples using pastebin
* Improved docs

## Version 0.0.0.9000

* Initial release

