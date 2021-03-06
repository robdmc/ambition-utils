Release Notes
=============

0.8.0
-----
* Refactored nested forms to simplify the api and make it more robust

BREAKING CHANGES (NestedFormMixin)

* No longer calls `form_save`. The base form and all mixin forms are required to have a `save` method
* Renamed `get_pre_save_method_kwargs` and `get_post_save_method_kwargs` to `get_nested_form_save_args`
* Removed `NestedModelFormMixin`, please use `NestedFormMixin` for all types of forms

0.6.1
-----
* Fixed bug with rrule future occurrences using time zones ahead of UTC

0.6.0
-----
* Added postgres lock app

0.4.0
-----
* Updated activity to include a reference to a context object and attributes to track completion as a ratio

0.3.0
-----
* Use tox to test more versions

0.2.0
-----
* Added mixin for tasks to add progress tracking

0.1.2
-----
* Do not modify the same dict while iterating

0.1.1
-----
* Use form config class to more easily control and document arguments

0.1.0
-----
* This is the initial release of ambition-utils
