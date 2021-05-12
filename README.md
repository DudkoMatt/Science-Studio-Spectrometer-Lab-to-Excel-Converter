# Science Studio Spectrometer Lab to Excel Converter

This is a simple script for converting .lab files from spectrometer to .xslx Excel files.


## Installing dependencies

This script was tested on Python 3.9.4. All dependencies are listed in [requirements.txt](requirements.txt). Install them with the following command:

```shell
pip install -r requirements.txt
```


## Running script

1) Place all *.lab files into the same directory with the script;
2) Run script.py;
3) Processed data will be in the output.xlsx file.


## Important notes

As it is not the final version of the project, there are some important remarks:
- Lambda range by default is filtered to: [400, 700]
- Namings for pages are used from the last digits before .lab extension (For example: "document_650.lab" will be converted to "650"). If there are no digits, an exception will be raised
- There is a regexp filter for measurement namings. It is disabled by default. Can be changed in filter_vectors function -> naming_pattern parameter
