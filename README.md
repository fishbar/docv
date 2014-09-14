# docv

[for now, this is copyed from dox-foundation, rename and modify something](https://github.com/punkave/dox-foundation)

Use [dox](https://github.com/visionmedia/dox) to automatically generate beautiful html documentation.

## Installation
Install the module with: `npm install docv -g`

## Documentation
```
$ docx --help

  Usage: docv [options]

  Options:

    -h, --help                  output usage information
    -V, --version               output the version number
    -r, --raw                   output "raw" comments, leaving the markdown intact
    -d, --debug                 output parsed comments for debugging
    -t, --title <string>        The title of the library or program you are generating code for (eg: Express). Overrides default of "Documentation"
    -s, --source <source>       The folder(s) which should be parsed. Multiple folders should be comma separated
    -i, --ignore <directories>  Comma seperated list of directories to ignore. Overrides default of test, public, static, views, templates
    -T, --target <target>       The folder which will contain the results. Default: <process.cwd()>/docs
    --template <jade template>  The jade template file to use

  Examples:

    # stdin
    $ docv > myfile.html

    # operates over stdio
    $ docv --title "myFile documentation" < myfile.js > myfile.html

    # parse a whole folder
    $ docv --source lib --target docs
```

## License
Copyright (c) 2012 P'unk Avenue
Licensed under the MIT license.
