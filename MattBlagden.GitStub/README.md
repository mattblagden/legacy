# GitStub

GitStub is a commandline utility to filter a Git repository.

GitStub parses an existing repository and writes a filtered representation of the original. The new repository contains all the same commits as the source repository, but only includes file contents for files whose path matches a user-specified whitelist. The content of files not on the whitelist is replaced with a short hexadecimal value.

Because of the way Git works, this operation must generate an entirely new repository: replacing the content of a file changes its hash, which changes the hash of its parent directory, which changes the hash of all directories above it, which changes the hash of the commit, which changes the hash of all commits that follow, and so on. Although a new repository is generated, it's done in a deterministic manner. This makes the output suitable to be pushed to a remote location, as the only parts that differ between invocations will be new commits.
