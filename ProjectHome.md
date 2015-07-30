## What ##

It is a simple python script with a simple command line interface that creates PDF booklets from another PDF by reordering its pages.

For example: A PDF with 4 pages: 1234 is reordered to 4123.

If then you print this pages to a paper two on the front and two on the back and fold it, you have a small book.

## Why ##

Because I wasn't able to find a FREE program that creates booklets from PDF files.

## Usage ##

```
# booklet-maker --help
Usage: bookletMaker [options] <input-pdf-file>
        Makes a booklet from the input PDF file by reordering its pages.

        Options:
            -d  --debug             Prints debug messages.
            -s  --size=<size>       Splits into booklets of the defined size.
            -o  --output=<file>     Define the output file.
            -f  --force             Overrides output file if necessary.
            -r  --range=<form>:<to> Selects range to make booklets.
                --from=<n>          Lower bound value for range (see --range).
                --to=<n>            Upper bound value for range (see --range).

       bookletMaker [-h|--help]
            Prints this text.

       bookletMaker [-v|--version]
            Prints version.

```

## Dependencies ##

  * **[Python](http://www.python.org/)** because it's a python script.
  * **[pyPdf](http://pybrary.net/pyPdf/)** a simple library to manipulate PDF files. (run _easy\_install pyPdf_)