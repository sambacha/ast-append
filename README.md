# ast-append 

> npm install ast-append

## Overview

walks an `abstract syntax tree` to append a non-enumberable property to each node

### Example

```javascript
require('ast-append')(ast)

var esprima = require('esprima')
var fs = require('fs')

var src = fs.readFileSync(__filename, 'utf8')
var ast = esprima.parse(src)

parents(ast)

ast.body[0].parent === ast.body
```

### License 

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.