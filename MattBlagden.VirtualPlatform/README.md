# Virtual Platform

This assembly exposes managed versions of the APIs provided by all `CIL Translator` target platforms.

The base directory contains the virtual platform interfaces. The sub-directories contain mappings to specific OS APIs, so applications can be run on development machines before translation to the target platform.

This assembly is simply something to link and run against during development, and is not translated by `CIL Translator`. These APIs are implemented separately for each platform.
