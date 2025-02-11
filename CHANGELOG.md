Change Log
==========

Version 1.2.0 *(2019-05-30)*
----------------------------

 * `Bridge` can now save the state of `View` objects. You may now optionally provide a `ViewSavedStateHandler` to `Bridge.initialize` in order to unlock this functionality.
 * Improved performance during configuration changes and when navigating while apps are in the foreground.

Version 1.1.3 *(2018-10-08)*
----------------------------

 * `Bridge.clear` is now safe to call in `Activity.onDestroy` when "Don't Keep Activities" is enabled.
 * All data is now correctly cleared on fresh launches for apps that do not use `Bridge` in every `Activity`.
 * Min SDK is now 14.

Version 1.1.2 *(2018-06-04)*
----------------------------

 * Data will no longer be automatically cleared for objects that go out of memory while an app is running. It is now more strongly recommended to use the `clear` method to manually delete data for objects in the process of being discarded.

Version 1.1.1 *(2017-08-17)*
----------------------------

 * Fixed `clear` behavior for a removed `Fragment` in the backstack.

Version 1.1.0 *(2017-08-16)*
----------------------------

 * Added support for saving Bitmaps.
 * Improved automatic clearing of old data.
 * Added `clear` method for manually clearing data from disk for a given object.
 * Added `clearAll` method for manually clearing all data from disk associated with `Bridge`.

Version 1.0.0 *(2017-06-22)*
----------------------------

Initial release.