# physicript CV related repo

Helper `data`, `functions`, and test `images` for computer-vision related tasks - by [appcubic](https://www.appcubic.com/)

## How to get the url from this repo

- `./raw-data/yolo_80_classes.json` can be accessed via`https://raw.githubusercontent.com/physicrypt/physicript-computer-vison-helpers/main/raw-data/yolo_80_classes.json`

Using `python`
```python
import urllib.request, json
json_url = "https://raw.githubusercontent.com/physicrypt/physicript-computer-vison-helpers/main/raw-data/yolo_80_classes.json"
data = {}
with urllib.request.urlopen(json_url) as url_return:
    data = json.load(url_return)
    data = {int(key):val for key, val in data.items()}
```