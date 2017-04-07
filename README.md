# api documentation for  [sse (v0.0.6)](https://github.com/einaros/sse.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-sse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sse)
#### The HTML5 Server-Sent events specification is introduced "to enable servers to push data to Web pages over HTTP or using dedicated server-push protocols".

[![NPM](https://nodei.co/npm/sse.png?downloads=true)](https://www.npmjs.com/package/sse)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sse/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sse_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sse/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sse/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sse/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Einar Otto Stangvik",
        "email": "einaros@gmail.com",
        "url": "http://2x.io"
    },
    "bugs": {
        "url": "https://github.com/einaros/sse.js/issues"
    },
    "dependencies": {
        "options": "latest"
    },
    "description": "The HTML5 Server-Sent events specification is introduced \"to enable servers to push data to Web pages over HTTP or using dedicated server-push protocols\".",
    "devDependencies": {
        "expect.js": "latest",
        "mocha": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "3192461dfa38c78424dd9bf8ea025619a125aa10",
        "tarball": "https://registry.npmjs.org/sse/-/sse-0.0.6.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "gitHead": "8bba85fb615920a2aefa431992e8b44dd89ccf72",
    "homepage": "https://github.com/einaros/sse.js",
    "keywords": [
        "real-time",
        "server-sent-events",
        "html5",
        "sse",
        "messaging"
    ],
    "maintainers": [
        {
            "name": "einaros",
            "email": "einaros@gmail.com"
        }
    ],
    "name": "sse",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/einaros/sse.js.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "0.0.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sse](#apidoc.module.sse)
1.  [function <span class="apidocSignatureSpan">sse.</span>Client (req, res)](#apidoc.element.sse.Client)
1.  [function <span class="apidocSignatureSpan">sse.</span>super_ ()](#apidoc.element.sse.super_)
1.  object <span class="apidocSignatureSpan">sse.</span>Client.prototype

#### [module sse.Client](#apidoc.module.sse.Client)
1.  [function <span class="apidocSignatureSpan">sse.</span>Client (req, res)](#apidoc.element.sse.Client.Client)
1.  [function <span class="apidocSignatureSpan">sse.Client.</span>super_ ()](#apidoc.element.sse.Client.super_)

#### [module sse.Client.prototype](#apidoc.module.sse.Client.prototype)
1.  [function <span class="apidocSignatureSpan">sse.Client.prototype.</span>close ()](#apidoc.element.sse.Client.prototype.close)
1.  [function <span class="apidocSignatureSpan">sse.Client.prototype.</span>initialize ()](#apidoc.element.sse.Client.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">sse.Client.prototype.</span>send (event, data, id)](#apidoc.element.sse.Client.prototype.send)



# <a name="apidoc.module.sse"></a>[module sse](#apidoc.module.sse)

#### <a name="apidoc.element.sse.Client"></a>[function <span class="apidocSignatureSpan">sse.</span>Client (req, res)](#apidoc.element.sse.Client)
- description and source-code
```javascript
function SSEClient(req, res) {
  this.req = req;
  this.res = res;
  var self = this;
  res.on('close', function() {
    self.emit('close');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sse.super_"></a>[function <span class="apidocSignatureSpan">sse.</span>super_ ()](#apidoc.element.sse.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sse.Client"></a>[module sse.Client](#apidoc.module.sse.Client)

#### <a name="apidoc.element.sse.Client.Client"></a>[function <span class="apidocSignatureSpan">sse.</span>Client (req, res)](#apidoc.element.sse.Client.Client)
- description and source-code
```javascript
function SSEClient(req, res) {
  this.req = req;
  this.res = res;
  var self = this;
  res.on('close', function() {
    self.emit('close');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sse.Client.super_"></a>[function <span class="apidocSignatureSpan">sse.Client.</span>super_ ()](#apidoc.element.sse.Client.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sse.Client.prototype"></a>[module sse.Client.prototype](#apidoc.module.sse.Client.prototype)

#### <a name="apidoc.element.sse.Client.prototype.close"></a>[function <span class="apidocSignatureSpan">sse.Client.prototype.</span>close ()](#apidoc.element.sse.Client.prototype.close)
- description and source-code
```javascript
close = function () {
  this.res.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sse.Client.prototype.initialize"></a>[function <span class="apidocSignatureSpan">sse.Client.prototype.</span>initialize ()](#apidoc.element.sse.Client.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
  this.req.socket.setNoDelay(true);
  this.res.writeHead(200, {
    'Content-Type': 'text/event-stream',
    'Cache-Control': 'no-cache',
    'Connection': 'keep-alive'
  });
  this.res.write(':ok\n\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sse.Client.prototype.send"></a>[function <span class="apidocSignatureSpan">sse.Client.prototype.</span>send (event, data, id)](#apidoc.element.sse.Client.prototype.send)
- description and source-code
```javascript
send = function (event, data, id) {
  if (arguments.length === 0) return;

  var senderObject = {
    event : event || undefined,
    data  : data || undefined,
    id    : id || undefined,
    retry : undefined
  };

  if (typeof event == 'object') {
    senderObject.event   = event.event || undefined,
    senderObject.data    = event.data || undefined,
    senderObject.id      = event.id || undefined,
    senderObject.retry   = event.retry || undefined
  }

  if (typeof event != 'object' && arguments.length === 1) {
    senderObject.event   = undefined;
    senderObject.data    = event;
  }

  if (senderObject.event) this.res.write('event: ' + senderObject.event + '\n');
  if (senderObject.retry) this.res.write('retry: ' + senderObject.retry + '\n');
  if (senderObject.id) this.res.write('id: ' + senderObject.id + '\n');

  senderObject.data = senderObject.data.replace(/(\r\n|\r|\n)/g, '\n');
  var dataLines = senderObject.data.split(/\n/);

  for (var i = 0, l = dataLines.length; i < l; ++i) {
    var line = dataLines[i];
    if ((i+1) === l) this.res.write('data: ' + line + '\n\n');
    else this.res.write('data: ' + line + '\n');
  }
}
```
- example usage
```shell
...
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('okay');
});

server.listen(8080, '127.0.0.1', function() {
  var sse = new SSE(server);
  sse.on('connection', function(client) {
    client.send('hi there!');
  });
});
'''

Client code for the above server:

'''js
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
