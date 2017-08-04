mosc-curated-list

This repository is the primary data source for the curated app. It has a client and a server. It is live at curated.bvpmosc.tech.

The goal is to have few high-quality choices so that developpers can quickly find the best package for their need. Only a handful of packages will be accepted for each category.

The list of curated packages are written in the PACKAGES.md markdown file. This file contains the data in a special format design to be still easily readable without parser.

Contributing

This package list is open to contribution! 👍

To contribute, open a PR by editing the PACKAGES.md file and read the following guide.

You can also contribute to the client app and the graphql server!

How to add a category

Each category is represented by a level-1 title and contains the packages until the next title.

Example:

# Category label
How to add a package

A package is a bullet-point line followed by some fields formatted in a particualiar way. It will be parsed by the mosc-curated app.

The row just starts with a link to the package repository, whose label is used as the package name in the app.

Each field is separated by a comma , and the value is put after colons :.

Example:

- [name](link), field1:value, field2:value, field3:value
Some fields can contain a list of values which are separated by a pipe | (without spaces).

Example:

array_field:value1|value2|value3
Supported fields

The package fields currently supported are: Source

Tags (array): list of supported Vue major versions. Example: Tags:os|js. 
links (array): list of useful links. Example: links:[doc](https://doc.com/)|[demo](https://demo.com/).
status: developpement status. Values: dev or stable. Example: status:stable.
badge: special badge. Recommended values: official. Example: badge:official.
Example

# Core

- [mosc-curated](https://github.com/bvpmosc/mosc-curated), Tags:official|js, links:[website](https://bvpmosc.tech/)|[eventinsta](https://github.com/BVPMOSC/EventInsta), badge:official, status:stable