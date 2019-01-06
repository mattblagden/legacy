# MergeJS

MergeJS is a simple tool that will concatenate files according to a merge list, using only node.js, instead of any platform-specific script.

MergeJS accepts a single argument: the path to a folder containing a merge list.

The merge list is the file named "merge" in the specified folder. The first line of the file specifies the output filename. Each subsequent line is a relative path to a file to be concatenated. All files are assumed to have ".js" extensions.

## Example

Given the following files:

```
/project/README.md
/project/merge
/project/one.js
/project/stuff/three.js
/project/two.js
```

And `/project/merge` containing:

```
output

src/one
two
stuff/three
```

Running MergeJS with the argument `/project` would produce a file at `/project/output.js` containing `one.js`, followed by `two.js`, followed by `three.js`.
