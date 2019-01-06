# Portable Executable

A library for generating and parsing native and managed Portable Executable images.

The project consists of three main namespaces:

* `PortableExecutable` - A hierarchy of objects that represent each part of the Portable Executable format. The native instruction stream is left as a blob; parsing/generation of instructions is handled by other libraries.
* `PortableExecutable.Managed` - A hierarchy of objects that represent the managed part of the image. All heaps, tables, and instruction streams are fully parsed and represented.
* `PortableExecutable.Serialization` - Tools to convert between serialized Portable Executable images and the object hierarchies.
