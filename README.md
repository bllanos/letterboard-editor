# Letterboard text validator

**Project started Spring 2020**

**Bernard Llanos**

## Problem description

Suppose an organization has a large letterboard for advertising, such as shown in the picture below:

![A community letterboard](./docs/img/physical_letterboard.jpg)

Coordinating changes to the text on the letterboard is complicated by constraints:
- There is a limited inventory of cards of each letter
- The letterboard imposes limits on the lengths of lines of letters

This repository contains programs for helping people compose text that will meet the constraints of a letterboard.

## Letterboard text validator webpage

The webpage, [html/index.html](./html/index.html) is a self-contained program that lets users enter text to be displayed on a letterboard, and then validates the text, displaying warnings if the text does satisfy all constraints.

It requires only a web browser to use, so that it can be distributed to people who cannot set up a web server or any software development tools. To use the webpage, open it in a web browser while connected to the Internet. (An Internet connection is required since the webpage loads the JavaScript libraries that it depends on from the Internet.)

## Development notes

- The JSON files in the root directory of the repository are reference files for the inventory of letters for a letterboard, and are not part of the source code of any programs.
- [html/index.html](./html/index.html) contains copies of the contents of the JSON files in a series of constants at the top of its internal script. To change the inventory of letters, or the properties of the letterboard, as used by the webpage, modify these constants.