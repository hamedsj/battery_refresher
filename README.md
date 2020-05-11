# battery_refresher
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A package that refresh battery info every n second

## Usage

1. **Clone files into your system**

```bash
git clone https://github.com/hamedsj/battery_refresher
```

2. **Make files executable**

```bash
chmod +x battery_refresher.py cron_script.sh
```

3. **Add cron_script to run on every reboot**
```bash
sudo crontab -e
```
  and add this line to end of the table
```bash
@reboot /path/of/repo/cron_script.sh
```

## Change timeout of battery info refresh
For changing time of refresh, open `cron_script.sh` file and change argument of python script
```bash
#!/bin/bash

#change 30 to everything (second) you want
python3 /path/of/repo/battery_refresher.py 30
```
## License
The MIT License

Copyright (c) 2010-2020 Google, Inc. http://angularjs.org

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
