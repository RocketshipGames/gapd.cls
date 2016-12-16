# GAPD LaTeX Class File

This is a more proper LaTeX class file for the Game and Puzzle Design
Journal.  It is derived from the original manually included command
definitions, but simplifies the actual content document template.

## Changes

Among the improvements from the article writer's perspective:

 * Instead of manually providing the slightly different syntax for the
   main author listing, citation author list, and page header author
   list, these are all computed from a simple \Author{}{} command.  It
   will properly present first initial and last name in the order
   appropriate to each use, conjoin two authors with a single "and",
   and with multiple authors use an Oxford-comma list in the
   bibliographic statement but "First et al."  in the header.

 * The two column format is done without using multicol, so that the
   latter doesn't have to be continually opened and closed for
   figures, etc..  As a consequence, the latter should just be done
   with the usual floats and the command macros have been removed.
   This does mean LaTeX will place them in slightly different
   locations that the original commands did, but it should mostly be
   allowed to do so.  E.g., it's usually poor form to have a figure on
   the first page, so LaTeX will not do that unless forced.

 * The sample article has been corrected in some but not all ways to
   use proper TeX commands and hints for ranges versus em dashes,
   unbreakable spaces before numbers, and so on.

## To-Do

Items that remain to be done include:

  * Adapt journal production scripts to compile multiple documents,
    properly resetting metadata and setting page numbers for each.
  
  * Potentially move the sample article and graphics to a subfolder or
    separate repo so the graphics aren't included in the TeX inputs
    path.  Replace with a more conventional self-documenting example.

## Changelog

* Converted to LaTeX class by Joe Kopena, 2016/12/15
* Original styling by Cameron Browne, 2014/09/11

## License

## License

This class package is provided under the open source
[MIT license](http://opensource.org/licenses/MIT):

> The MIT License (MIT)
>
> Permission is hereby granted, free of charge, to any person
> obtaining a copy of this software and associated documentation files
> (the "Software"), to deal in the Software without restriction,
> including without limitation the rights to use, copy, modify, merge,
> publish, distribute, sublicense, and/or sell copies of the Software,
> and to permit persons to whom the Software is furnished to do so,
> subject to the following conditions:
>
> The above copyright notice and this permission notice shall be
> included in all copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
> EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
> NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
> BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
> ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
> CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.
