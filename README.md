# mw_sample_downloader
Simple python script to search for samples by hash on various malware repos and download a copy locally for analysis

Currently supports the following repos:
  - VirusSign
  - VirusShare (requires that you have your own login credentials)
  - VirusTotal (requires that you have a private API key)
  
WIP integrations:
  - Viper Malware Archive

USAGE:
malware_dl.py [-h] -f FILE [-o OUT] [-v] [-d]

optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE
  -o OUT, --out OUT     Specifies folder path to download files to. If not
                        present, default is ./downloads/
  -v, --verbose
  -d, --debug


Configuration:
  - Priority values: Each configured and enabled repo will need to have a priority value assigned to it. This value determines the order each repo is queried against. 
  - All other items of note are documented within the conf file
