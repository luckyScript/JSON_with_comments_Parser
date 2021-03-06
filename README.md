# JSON_with_comments_Parser

![](https://travis-ci.com/luckyscript/json_parser.svg?branch=master)
[![Coverage Status](https://coveralls.io/repos/github/luckyscript/json_parser/badge.svg?branch=master)](https://coveralls.io/github/luckyscript/json_parser?branch=master)

## use

```sh
npm install json_with_comments_parser

import { parse } from 'json_with_comments_parser'

parse('{"a": "b"}')
```

## examples
```js
parse(`{
            "a":"b" //comment
        }`);

result: 
{ 
    value: [
        { 
            "key": "a",
            "children":[],
            "value":"b",
            "type":"String",
            "comment":"comment"
        }
    ],
    type: 'Object'
}
```

## TODO:
[ ] throw Exception friendly

# LICENSE

---

The MIT License (MIT)

Copyright (c) 2015 Kay Lu <main.lukai@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

