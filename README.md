# KK Pickit Editor

## How to use

1 - Install the latest version of [Python](https://www.python.org/ftp/python/3.11.3/python-3.11.3-amd64.exe) for your system\
2 - Open kkpickit.py with vscode or whatever you like to edit with\
3 - Set the path to your save folder at the top of the file\
3 - Enable items by changing "enabled":0 to 1, along with the sockets etc\
4 - For more complex items, the filter format is as follows
```json
"filters":{
    "FilterOne":{"min":1,"stats":{
        "damagepercent":{"req":1,"val1":">200"},
    }},
    "FilterTwo":{"min":1,"stats":{
        "damagepercent":{"req":1,"val1":">269"},
    }},
},
```
5 - Filter names can be up to 20 characters long\
6 - "min" is how many stats in the filter needs to match\
7 - "req" is if the specific stat is required\
8 - Valid operators are >, <, =, -\
9 - Here's an example of a stat with a specific skill `"plusclassskill1":{"req":1,"val1":">2","val2":"-271"},` where 271 is the skill id from the game tables\
10 - All the stat aliases/names are listed in the `modifiers` array\
\
Run via the cmd or by double clicking the .py

Enjoy!