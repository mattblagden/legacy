# Git

A collection of tools for inspecting and generating Git repositories. The library currently provides read-only access to existing Git repositories, and can write new repositories.

There are two main components:

* The `Repository` class provides access to all of the Git objects (branches, commits, directory trees, files, etc.)
* The `RepositoryNavigator` class acts as a reader to provide easy access to aggregate information, such as retrieving the contents of a file at a specific commit, or listing the hierarchy of files and their most recent changes at a specific commit.
