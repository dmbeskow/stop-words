## Stop words JSON

This is a JSON file that I use for several projects.  99% of this file is taken from [https://github.com/6/stopwords-json](https://github.com/6/stopwords-json)

## Usage

The following code loads a stop-words dictionary in Python3

```python
import json
import urllib.request
link = "https://raw.githubusercontent.com/dmbeskow/stop-words/master/stopwords-all.json"
with urllib.request.urlopen(link) as url:
    stop_dict = json.loads(url.read().decode())
```
