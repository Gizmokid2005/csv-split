#CSV Split

Developed and tested on Ruby 2.4.0

A ruby script that splits a large csv file into smaller files and stores the smaller files into the ```converted-files``` directory.

This script has eight (8) parameters:

```
Options:
  --file-path=<s>                            Path to csv file to be split
  --new-file-name=<s>                        Name of the new files. This will be appended with an incremented number
                                             (default: split)
  --split-path-name=<s>                      Folder to save the new files in (default: converted-files)
  --include-headers, --no-include-headers    Include headers in new files (default: true)
  --line-count=<i>                           Number of lines to output per file (default: 1)
  --delimiter=<s>                            Column delimiter (separation character) (default: ,)
  --remove-columns                           Specify column names to be removed during processing in remove.csv
  --help, -h:   Show this message
```

## Required Gems
- optimist

## Installation

1. Clone repository
2. Install required gem (or use bundler via ```bundle install```):
		
	``` 
	gem install optimist 
	```

## Running the script

```
ruby csv-split.rb --file-path path/to/csv/file/.csv --line-count 2500 --include-headers

```

