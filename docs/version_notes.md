Version notes
=====================

<!-- ---
layout: docs
title: Version Notes
description: List of version notes
redirect_from: "/version_notes/"
--- -->

### Versions 3.*
* :green_book: log4stash 3.0.0 targets .net standard natively, removed RestSharp dependency and added API Key authentication

### Versions 2.*

* :green_book: log4stash 2.0.4 has new filters see [filters section][filters-section] for more information. Added support for AWS Version 4 authorization header thanks to [@Marcelo Palladino][mfpalladino]. Support configuring multiple elastic nodes. Add document id source so you can decide your own doc id (instead of getting generated one from the elastic). Add Timeout option for requests. Many thanks to [@eran gil][erangil] for the efforts and the pull requests.

* :green_book: log4stash 2.0.0 has new filter `Json`, you can add it if you have json string in you log event and you want it to be converted to an object and not be passed as string to the elastic. Thanks to [@Ignas Velža][ignasv] for this filter.

### Versions 1.*

* :green_book: log4stash 1.1.0 has new feature `SerializeObjects`, if true (the default) it serializes the exception object and message object into json object and add them to Elastic. You can see them under "MessageObject" and "ExceptionObject" keys.  - [Related commit](https://github.com/urielha/log4stash/commit/560676de9b074be70e00f93566c543a846ba5c8e)


### see also 
* [Breaking changes](https://github.com/urielha/log4stash/blob/master/docs/breaking.md)


[ignasv]:https://github.com/ignasv
[erangil]:https://github.com/erangil2
[mfpalladino]:https://github.com/mfpalladino

[filters-section]:https://github.com/urielha/log4stash#filters
