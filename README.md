# RawClicksTool

Bash script that allows you to pull, merge and filter raw click logs.

### Dependencies

The tool depends on basic GNU shell programs as well as jq and curl.

- jq [Download](https://stedolan.github.io/jq/)
- zip
- awk
- sort
- curl [Download](https://curl.haxx.se/)
- wget

## Usage

`./clicktool`

You will be prompt for the following information:

- api key
- from date (yyyy-mm-dd)
- to date
- affiliate id (optional)

The program will then proceed to download all files in a temporary folder. This may take a while depending on your network connection and the number of clicks ran in the selected period of time. Once downloaded, the program will merge and sort all the files into a single one.

Once this is done, you will be prompted for an optional filtering step. This filtering step is very basic and the only comparison operator supported is "equal". An example is to use this option if you want to filter for a particular offer id.

You will be prompt for 2 things:

- the csv field name
- the value you want to compare to

Once the optional filtering is done, the program will proceed to 
