  
# zip-crack
The purpose of this script is brute force ZIP archives that are password protected. 

The dictionary file passed as an argument can be whatever the user chooses. passwords.txt is included here in this repo.

The passwords.txt file that is a companion to this script is spefically designed for crimeware variants such as BokBot, Valak, Ursnif, and Dridex that are often delivered as ZIP archives.

Original zip-crack_v1 version is provided as it is faster if the regex method is unnecessary. The regex in v2 script will need to be modified for the particular use-case.

# Dependency:
Python3

pyzipper - See this documentation to install: https://pypi.org/project/pyzipper/

# Usage: 
v1
```sh
python3 zip-crack_v1.py -f EVILZIP.zip -d passwords.txt
```

v2 dictionary METHOD:
```sh
 python3 zip-crack.py -f '<FILENAME>.zip' -d -p passwords.txt
```
v2 regex METHOD: 
```sh
python3 zip-crack.py -f '<FILENAME>.zip' -r
```

# Acknowledgments: 
Special thanks to @AbsoZed, becuase I borrowed some of his code. 
