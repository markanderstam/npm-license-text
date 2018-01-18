# npm-license-text

Generate a text-file containing the licenses for all npm-modules
included in one or several projects.

Uses [npm-license-crawler](https://www.npmjs.com/package/npm-license-crawler)
to find all modules and their licenses.

**WARNING**: This module uses heuristics to find the license-text
for the modules. This may not work for all modules and
may produce the wrong license for some modules. You must check
the generated license file for correctness manually.

## Usage

    npm-license-text <startDir> <outputFile>

The startDir is sent to npm-license-crawler as a `start` option.
See the documentation of npm-license-crawler for more details.

The script exits with an error if it cannot guess the license for
one or more modules
