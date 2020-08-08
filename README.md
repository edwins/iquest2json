This script will read iRODS iquest formatted text from standard input and output the results as a json array.

To use:

    # wget https://raw.githubusercontent.com/edwins/iquest2json/master/iquest2json
    # chmod a+x iquest2json
    # iquest "..." | ./iquest2json

Example: 

    iquest "select count(DATA_ID) where COLL_NAME like '/tempZone/home/rods%'" | ./iquest2json
    {
      "results": [
        {
          "DATA_ID": "37642"
        }
      ]
    }

