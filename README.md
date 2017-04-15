# api documentation for  [amqp (v0.2.6)](https://github.com/postwait/node-amqp#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-amqp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-amqp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-amqp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-amqp)
#### AMQP driver for node

[![NPM](https://nodei.co/npm/amqp.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/amqp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-amqp/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-amqp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-amqp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-amqp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ryan Dahl"
    },
    "bugs": {
        "url": "http://github.com/postwait/node-amqp/issues"
    },
    "contributors": [
        {
            "name": "Vasili Sviridov"
        },
        {
            "name": "Theo Schlossnagle"
        },
        {
            "name": "Vincent Desjardins"
        },
        {
            "name": "Liang-Chi Hsieh"
        },
        {
            "name": "Tim Baga"
        },
        {
            "name": "Stéphane Alnet"
        },
        {
            "name": "Alen Mujezinovic"
        },
        {
            "name": "Michael Bridgen"
        },
        {
            "name": "Chris Bond"
        },
        {
            "name": "Andrei Vereha"
        },
        {
            "name": "Mike Bardzinski"
        },
        {
            "name": "James Carr"
        },
        {
            "name": "David Barshow"
        },
        {
            "name": "Jason Pincin"
        },
        {
            "name": "Carl Hörberg"
        }
    ],
    "dependencies": {
        "lodash": "^4.0.0"
    },
    "description": "AMQP driver for node",
    "devDependencies": {
        "longjohn": "~0.2.1",
        "optimist": "~0.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d97fee5143026fa0b4fd6a5d56485f0448eb37ca",
        "tarball": "https://registry.npmjs.org/amqp/-/amqp-0.2.6.tgz"
    },
    "gitHead": "1d30ce178d4a1781f2199f136e4e942e725cfa4c",
    "homepage": "https://github.com/postwait/node-amqp#readme",
    "keywords": [
        "amqp"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://github.com/postwait/node-amqp/raw/master/LICENSE-MIT"
        }
    ],
    "main": "./amqp",
    "maintainers": [
        {
            "name": "ry"
        },
        {
            "name": "postwait"
        }
    ],
    "name": "amqp",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/postwait/node-amqp.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.2.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module amqp](#apidoc.module.amqp)
1.  [function <span class="apidocSignatureSpan">amqp.</span>Connection (connectionArgs, options, readyCallback)](#apidoc.element.amqp.Connection)
1.  [function <span class="apidocSignatureSpan">amqp.</span>createConnection (options, implOptions, readyCallback)](#apidoc.element.amqp.createConnection)
1.  object <span class="apidocSignatureSpan">amqp.</span>Connection.prototype

#### [module amqp.Connection](#apidoc.module.amqp.Connection)
1.  [function <span class="apidocSignatureSpan">amqp.</span>Connection (connectionArgs, options, readyCallback)](#apidoc.element.amqp.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.</span>super_ ()](#apidoc.element.amqp.Connection.super_)

#### [module amqp.Connection.prototype](#apidoc.module.amqp.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_bodyToBuffer (body)](#apidoc.element.amqp.Connection.prototype._bodyToBuffer)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_chooseHost ()](#apidoc.element.amqp.Connection.prototype._chooseHost)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_createSocket ()](#apidoc.element.amqp.Connection.prototype._createSocket)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_getSSLOptions ()](#apidoc.element.amqp.Connection.prototype._getSSLOptions)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_inboundHeartbeatTimerReset ()](#apidoc.element.amqp.Connection.prototype._inboundHeartbeatTimerReset)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_onMethod (channel, method, args)](#apidoc.element.amqp.Connection.prototype._onMethod)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_outboundHeartbeatTimerReset ()](#apidoc.element.amqp.Connection.prototype._outboundHeartbeatTimerReset)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_parseURLOptions (connectionString)](#apidoc.element.amqp.Connection.prototype._parseURLOptions)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_saslResponse ()](#apidoc.element.amqp.Connection.prototype._saslResponse)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendBody (channel, body, properties)](#apidoc.element.amqp.Connection.prototype._sendBody)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendHeader (channel, size, properties)](#apidoc.element.amqp.Connection.prototype._sendHeader)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendMethod (channel, method, args)](#apidoc.element.amqp.Connection.prototype._sendMethod)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_startHandshake ()](#apidoc.element.amqp.Connection.prototype._startHandshake)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>addAllListeners ()](#apidoc.element.amqp.Connection.prototype.addAllListeners)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>connect ()](#apidoc.element.amqp.Connection.prototype.connect)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>disconnect ()](#apidoc.element.amqp.Connection.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>end ()](#apidoc.element.amqp.Connection.prototype.end)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>exchange (name, options, openCallback)](#apidoc.element.amqp.Connection.prototype.exchange)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>exchangeClosed (name)](#apidoc.element.amqp.Connection.prototype.exchangeClosed)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>generateChannelId ()](#apidoc.element.amqp.Connection.prototype.generateChannelId)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>heartbeat ()](#apidoc.element.amqp.Connection.prototype.heartbeat)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>publish (routingKey, body, options, callback)](#apidoc.element.amqp.Connection.prototype.publish)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>queue (name)](#apidoc.element.amqp.Connection.prototype.queue)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>queueClosed (name)](#apidoc.element.amqp.Connection.prototype.queueClosed)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>reconnect ()](#apidoc.element.amqp.Connection.prototype.reconnect)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>setImplOptions (options)](#apidoc.element.amqp.Connection.prototype.setImplOptions)
1.  [function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>setOptions (options)](#apidoc.element.amqp.Connection.prototype.setOptions)



# <a name="apidoc.module.amqp"></a>[module amqp](#apidoc.module.amqp)

#### <a name="apidoc.element.amqp.Connection"></a>[function <span class="apidocSignatureSpan">amqp.</span>Connection (connectionArgs, options, readyCallback)](#apidoc.element.amqp.Connection)
- description and source-code
```javascript
function Connection(connectionArgs, options, readyCallback) {
  EventEmitter.call(this);
  this.setOptions(connectionArgs);
  this.setImplOptions(options);

  if (typeof readyCallback === 'function') {
    this._readyCallback = readyCallback;
  }

  this.connectionAttemptScheduled = false;
  this._defaultExchange = null;
  this.channelCounter = 0;
  this._sendBuffer = new Buffer(maxFrameBuffer);

  this._blocked = false;
  this._blockedReason = null;
}
```
- example usage
```shell
...
      });
  });
});
'''

## Connection

'new amqp.Connection()' Instantiates a new connection. Use
'connection.connect()' to connect to a server.

'amqp.createConnection()' returns an instance of 'amqp.Connection', which contains
an instance of 'net.Socket' at its 'socket' property. All events and methods which work on
'net.Socket' can also be used on an 'amqp.Connection' instance. (e.g., the
events ''connect'' and ''close''.)
...
```

#### <a name="apidoc.element.amqp.createConnection"></a>[function <span class="apidocSignatureSpan">amqp.</span>createConnection (options, implOptions, readyCallback)](#apidoc.element.amqp.createConnection)
- description and source-code
```javascript
createConnection = function (options, implOptions, readyCallback) {
  var c = new Connection(options, implOptions, readyCallback);
  c.connect();
  return c;
}
```
- example usage
```shell
...
IMPORTANT: This module only works with node v0.4.0 and later.

An example of connecting to a server and listening on a queue.

'''javascript
var amqp = require('amqp');

var connection = amqp.createConnection({ host: 'dev.rabbitmq.com' });

// add this for better debuging
connection.on('error', function(e) {
  console.log("Error from amqp: ", e);
});

// Wait for connection to become established.
...
```



# <a name="apidoc.module.amqp.Connection"></a>[module amqp.Connection](#apidoc.module.amqp.Connection)

#### <a name="apidoc.element.amqp.Connection.Connection"></a>[function <span class="apidocSignatureSpan">amqp.</span>Connection (connectionArgs, options, readyCallback)](#apidoc.element.amqp.Connection.Connection)
- description and source-code
```javascript
function Connection(connectionArgs, options, readyCallback) {
  EventEmitter.call(this);
  this.setOptions(connectionArgs);
  this.setImplOptions(options);

  if (typeof readyCallback === 'function') {
    this._readyCallback = readyCallback;
  }

  this.connectionAttemptScheduled = false;
  this._defaultExchange = null;
  this.channelCounter = 0;
  this._sendBuffer = new Buffer(maxFrameBuffer);

  this._blocked = false;
  this._blockedReason = null;
}
```
- example usage
```shell
...
      });
  });
});
'''

## Connection

'new amqp.Connection()' Instantiates a new connection. Use
'connection.connect()' to connect to a server.

'amqp.createConnection()' returns an instance of 'amqp.Connection', which contains
an instance of 'net.Socket' at its 'socket' property. All events and methods which work on
'net.Socket' can also be used on an 'amqp.Connection' instance. (e.g., the
events ''connect'' and ''close''.)
...
```

#### <a name="apidoc.element.amqp.Connection.super_"></a>[function <span class="apidocSignatureSpan">amqp.Connection.</span>super_ ()](#apidoc.element.amqp.Connection.super_)
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



# <a name="apidoc.module.amqp.Connection.prototype"></a>[module amqp.Connection.prototype](#apidoc.module.amqp.Connection.prototype)

#### <a name="apidoc.element.amqp.Connection.prototype._bodyToBuffer"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_bodyToBuffer (body)](#apidoc.element.amqp.Connection.prototype._bodyToBuffer)
- description and source-code
```javascript
_bodyToBuffer = function (body) {
  // Handles 3 cases
  // - body is utf8 string
  // - body is instance of Buffer
  // - body is an object and its JSON representation is sent
  // Does not handle the case for streaming bodies.
  // Returns buffer.
  if (typeof(body) == 'string') {
    return [null, new Buffer(body, 'utf8')];
  } else if (body instanceof Buffer) {
    return [null, body];
  } else {
    var jsonBody = JSON.stringify(body);

    debug && debug('sending json: ' + jsonBody);

    var props = {contentType: 'application/json'};
    return [props, new Buffer(jsonBody, 'utf8')];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._chooseHost"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_chooseHost ()](#apidoc.element.amqp.Connection.prototype._chooseHost)
- description and source-code
```javascript
_chooseHost = function () {
  if(Array.isArray(this.options.host)){
    if(this.hosti == null){
      if(typeof this.options.hostPreference == 'number') {
        this.hosti = (this.options.hostPreference < this.options.host.length) ?
          this.options.hostPreference : this.options.host.length-1;
      } else {
        this.hosti = parseInt(Math.random() * this.options.host.length, 10);
      }
    } else {
      // If this is already set, it looks like we want to choose another one.
      // Add one to hosti but don't overflow it.
      this.hosti = (this.hosti + 1) % this.options.host.length;
    }
    return this.options.host[this.hosti];
  } else {
    return this.options.host;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._createSocket"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_createSocket ()](#apidoc.element.amqp.Connection.prototype._createSocket)
- description and source-code
```javascript
_createSocket = function () {
  var hostName = this._chooseHost(), self = this, port = this.options.port;
  var parsedHost = URL.parse(hostName);
  if(parsedHost.port){
    hostName = parsedHost.hostname;
    port = parsedHost.port;
  }

  var options = {
    port: port,
    host: hostName
  };

  // Disable tcp nagle's algo
  // Default: true, makes small messages faster
  var noDelay = this.options.noDelay || true;

  var resetConnectionTimeout = function () {
    debug && debug('connected so resetting connection timeout');
    this.setTimeout(0);
  };

  // Connect socket
  if (this.options.ssl.enabled) {
    debug && debug('making ssl connection');
    options = _.assignIn(options, this._getSSLOptions());
    this.socket = tls.connect(options, resetConnectionTimeout);
  } else {
    debug && debug('making non-ssl connection');
    this.socket = net.connect(options, resetConnectionTimeout);
  }
  var connTimeout = this.options.connectionTimeout;
  if (connTimeout) {
    debug && debug('setting connection timeout to ' + connTimeout);
    this.socket.setTimeout(connTimeout, function () {
      debug && debug('connection timeout');
      this.destroy();
      var e = new Error('connection timeout');
      e.name = 'TimeoutError';
      self.emit('error', e);
    });
  }

  this.socket.setNoDelay(noDelay);

  // Proxy events.
  // Note that if we don't attach a 'data' event, no data will flow.
  var events = ['close', 'connect', 'data', 'drain', 'error', 'end', 'secureConnect', 'timeout'];
  _.forEach(events, function(event){
    self.socket.on(event, self.emit.bind(self, event));
  });

  // Proxy a few methods that we use / previously used.
  var methods = ['destroy', 'write', 'pause', 'resume', 'setEncoding', 'ref', 'unref', 'address'];
  _.forEach(methods, function(method){
    self[method] = function(){
      self.socket[method].apply(self.socket, arguments);
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._getSSLOptions"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_getSSLOptions ()](#apidoc.element.amqp.Connection.prototype._getSSLOptions)
- description and source-code
```javascript
_getSSLOptions = function () {
  if (this.sslConnectionOptions) return this.sslConnectionOptions;
  this.sslConnectionOptions = {};

  if (this.options.ssl.pfxFile) {
    this.sslConnectionOptions.pfx = fs.readFileSync(this.options.ssl.pfxFile);
  }
  if (this.options.ssl.keyFile) {
    this.sslConnectionOptions.key = fs.readFileSync(this.options.ssl.keyFile);
  }
  if (this.options.ssl.certFile) {
    this.sslConnectionOptions.cert = fs.readFileSync(this.options.ssl.certFile);
  }
  if (this.options.ssl.caFile) {
    if (Array.isArray(this.options.ssl.caFile)) {
      this.sslConnectionOptions.ca = this.options.ssl.caFile.map(function(f){
        return fs.readFileSync(f);
      });
    } else {
      this.sslConnectionOptions.ca = fs.readFileSync(this.options.ssl.caFile);
    }
  }

  this.sslConnectionOptions.rejectUnauthorized = this.options.ssl.rejectUnauthorized;
  this.sslConnectionOptions.passphrase = this.options.ssl.passphrase;

  return this.sslConnectionOptions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._inboundHeartbeatTimerReset"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_inboundHeartbeatTimerReset ()](#apidoc.element.amqp.Connection.prototype._inboundHeartbeatTimerReset)
- description and source-code
```javascript
_inboundHeartbeatTimerReset = function () {
  if (this._inboundHeartbeatTimer !== null) {
    clearTimeout(this._inboundHeartbeatTimer);
    this._inboundHeartbeatTimer = null;
  }
  if (this.options.heartbeat) {
    var self = this;
    var gracePeriod = 2 * this.options.heartbeat;
    this._inboundHeartbeatTimer = setTimeout(function () {
      if(self.socket.readable || self.options.heartbeatForceReconnect){
        self.emit('error', new Error('no heartbeat or data in last ' + gracePeriod + ' seconds'));
      }
    }, gracePeriod * 1000);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._onMethod"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_onMethod (channel, method, args)](#apidoc.element.amqp.Connection.prototype._onMethod)
- description and source-code
```javascript
_onMethod = function (channel, method, args) {
  debug && debug(channel + " > " + method.name + " " + JSON.stringify(args));

  // Channel 0 is the control channel. If not zero then delegate to
  // one of the channel objects.

  if (channel > 0) {
    if (!this.channels[channel]) {
      debug && debug("Received message on untracked channel.");
      return;
    }
    if (!this.channels[channel]._onChannelMethod) {
      throw new Error('Channel ' + channel + ' has no _onChannelMethod method.');
    }
    this.channels[channel]._onChannelMethod(channel, method, args);
    return;
  }

  // channel 0

  switch (method) {
    // 2. The server responds, after the version string, with the
    // 'connectionStart' method (contains various useless information)
    case methods.connectionStart:
      // We check that they're serving us AMQP 0-9
      if (args.versionMajor !== 0 && args.versionMinor != 9) {
        this.socket.end();
        this.emit('error', new Error("Bad server version"));
        return;
      }
      this.serverProperties = args.serverProperties;
      // 3. Then we reply with StartOk, containing our useless information.
      this._sendMethod(0, methods.connectionStartOk, {
        clientProperties: this.options.clientProperties,
        mechanism: this.options.authMechanism,
        response: this._saslResponse(),
        locale: 'en_US'
      });
      break;

    // 4. The server responds with a connectionTune request
    case methods.connectionTune:
      if (args.frameMax) {
          debug && debug("tweaking maxFrameBuffer to " + args.frameMax);
          maxFrameBuffer = args.frameMax;
          this._sendBuffer = new Buffer(maxFrameBuffer);
          this.parser.setMaxFrameBuffer(maxFrameBuffer);
      }
      if (args.channelMax) {
          debug && debug("tweaking channelMax to " + args.channelMax);
          channelMax = args.channelMax;
      }
      // 5. We respond with connectionTuneOk
      this._sendMethod(0, methods.connectionTuneOk, {
        channelMax: channelMax,
        frameMax: maxFrameBuffer,
        heartbeat: this.options.heartbeat || 0
      });
      // 6. Then we have to send a connectionOpen request
      this._sendMethod(0, methods.connectionOpen, {
        virtualHost: this.options.vhost
        // , capabilities: ''
        // , insist: true
        ,
        reserved1: '',
        reserved2: true
      });
      break;


    case methods.connectionOpenOk:
      // 7. Finally they respond with connectionOpenOk
      // Whew! That's why they call it the Advanced MQP.
      if (this._readyCallback) {
        this._readyCallback(this);
        this._readyCallback = null;
      }
      this.emit('ready');
      break;

    case methods.connectionClose:
      var e = new Error(args.replyText);
      e.code = args.replyCode;
      if (!this.listeners('close').length) {
        console.log('Unhandled connection error: ' + args.replyText);
      }
      this.socket.destroy(e);
      break;

    case methods.connectionCloseOk:
      debug && debug("Received close-ok from server, closing socket");
      this.socket.end();
      break;

    case methods.connectionBlocked:
      debug && debug('Received connection.blocked from server with reason: ' + args.reason);
      this._blocked = true;
      this._blockedReason = args.reason;
      this.emit('blocked');
      break;

    case methods.connectionUnblocked:
      debug && debug('Received connection.unblocked from server');
      this._blocked = false;
      this._blockedReason = null;
      this.emit('unblocked');
      break;

    default:
      throw new Error("Uncaught method '" + method.name + "' with args " +
          JSON.stringify(args));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._outboundHeartbeatTimerReset"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_outboundHeartbeatTimerReset ()](#apidoc.element.amqp.Connection.prototype._outboundHeartbeatTimerReset)
- description and source-code
```javascript
_outboundHeartbeatTimerReset = function () {
  if (this._outboundHeartbeatTimer !== null) {
    clearTimeout(this._outboundHeartbeatTimer);
    this._outboundHeartbeatTimer = null;
  }
  if (this.socket.writable && this.options.heartbeat) {
    var self = this;
    this._outboundHeartbeatTimer = setTimeout(function () {
      self.heartbeat();
      self._outboundHeartbeatTimerReset();
    }, 1000 * this.options.heartbeat);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._parseURLOptions"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_parseURLOptions (connectionString)](#apidoc.element.amqp.Connection.prototype._parseURLOptions)
- description and source-code
```javascript
_parseURLOptions = function (connectionString) {
  var opts = {};
  opts.ssl = {};
  var url = URL.parse(connectionString);
  var scheme = url.protocol.substring(0, url.protocol.lastIndexOf(':'));
  if (scheme != 'amqp' && scheme != 'amqps') {
    throw new Error('Connection URI must use amqp or amqps scheme. ' +
                    'For example, "amqp://bus.megacorp.internal:5766".');
  }
  opts.ssl.enabled = ('amqps' === scheme);
  opts.host = url.hostname;
  opts.port = url.port || defaultPorts[scheme];
  if (url.auth) {
    var auth = url.auth.split(':');
    auth[0] && (opts.login = auth[0]);
    auth[1] && (opts.password = auth[1]);
  }
  if (url.pathname) {
    opts.vhost = unescape(url.pathname.substr(1));
  }
  return opts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._saslResponse"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_saslResponse ()](#apidoc.element.amqp.Connection.prototype._saslResponse)
- description and source-code
```javascript
_saslResponse = function () {
  var response;
  if (this.options.authMechanism == 'AMQPLAIN')
    response = {
      LOGIN: this.options.login,
      PASSWORD: this.options.password
    };
  else if (this.options.authMechanism == 'PLAIN')
    response = "\0" + this.options.login + "\0" + this.options.password;
  else if (this.options.authMechanism == 'EXTERNAL')
    response = "\0";
  else if (this.options.authMechanism == 'ANONYMOUS')
    response = "\0";
  else
    response = this.options.response;

  return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._sendBody"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendBody (channel, body, properties)](#apidoc.element.amqp.Connection.prototype._sendBody)
- description and source-code
```javascript
_sendBody = function (channel, body, properties) {
  var r = this._bodyToBuffer(body);
  var props = r[0], buffer = r[1];

  properties = _.assignIn(props || {}, properties);

  this._sendHeader(channel, buffer.length, properties);

  var pos = 0, len = buffer.length;
  var metaSize = 8; // headerBytes = 7, frameEndBytes = 1
  var maxBodySize = maxFrameBuffer - metaSize;

  while (len > 0) {
    var bodySize = len < maxBodySize ? len : maxBodySize;
    var frameSize = bodySize + metaSize;

    var b = new Buffer(frameSize);
    b.used = 0;
    b[b.used++] = 3; // constants.frameBody
    serializer.serializeInt(b, 2, channel);
    serializer.serializeInt(b, 4, bodySize);
    buffer.copy(b, b.used, pos, pos+bodySize);
    b.used += bodySize;
    b[b.used++] = 206; // constants.frameEnd;
    this.write(b);

    len -= bodySize;
    pos += bodySize;
  }
  return;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._sendHeader"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendHeader (channel, size, properties)](#apidoc.element.amqp.Connection.prototype._sendHeader)
- description and source-code
```javascript
_sendHeader = function (channel, size, properties) {
  var b = new Buffer(maxFrameBuffer); // FIXME allocating too much.
                                      // use freelist?
  b.used = 0;

  var classInfo = classes[60]; // always basic class.

  // 7 OCTET FRAME HEADER

  b[b.used++] = 2; // constants.frameHeader

  serializer.serializeInt(b, 2, channel);

  var lengthStart = b.used;

  serializer.serializeInt(b, 4, 0 /*dummy*/); // length

  var bodyStart = b.used;

  // HEADER'S BODY

  serializer.serializeInt(b, 2, classInfo.index);   // class 60 for Basic
  serializer.serializeInt(b, 2, 0);                 // weight, always 0 for rabbitmq
  serializer.serializeInt(b, 8, size);              // byte size of body

  // properties - first propertyFlags
  properties = _.defaults(properties || {}, {contentType: 'application/octet-stream'});
  var propertyFlags = 0;
  for (var i = 0; i < classInfo.fields.length; i++) {
    if (properties[classInfo.fields[i].name]) propertyFlags |= 1 << (15-i);
  }
  serializer.serializeInt(b, 2, propertyFlags);
  // now the actual properties.
  serializer.serializeFields(b, classInfo.fields, properties, false);

  //serializeTable(b, properties);

  var bodyEnd = b.used;

  // Go back to the header and write in the length now that we know it.
  b.used = lengthStart;
  serializer.serializeInt(b, 4, bodyEnd - bodyStart);
  b.used = bodyEnd;

  // 1 OCTET END

  b[b.used++] = 206; // constants.frameEnd;

  var s = new Buffer(b.used);
  b.copy(s);

  //debug && debug('header sent: ' + JSON.stringify(s));

  this.write(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._sendMethod"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_sendMethod (channel, method, args)](#apidoc.element.amqp.Connection.prototype._sendMethod)
- description and source-code
```javascript
_sendMethod = function (channel, method, args) {
  debug && debug(channel + " < " + method.name + " " + JSON.stringify(args));
  var b = this._sendBuffer;
  b.used = 0;

  b[b.used++] = 1; // constants.frameMethod

  serializer.serializeInt(b, 2, channel);

  var lengthIndex = b.used;

  serializer.serializeInt(b, 4, 42); // replace with actual length.

  var startIndex = b.used;


  serializer.serializeInt(b, 2, method.classIndex); // short, classId
  serializer.serializeInt(b, 2, method.methodIndex); // short, methodId

  serializer.serializeFields(b, method.fields, args, true);

  var endIndex = b.used;

  // write in the frame length now that we know it.
  b.used = lengthIndex;
  serializer.serializeInt(b, 4, endIndex - startIndex);
  b.used = endIndex;

  b[b.used++] = 206; // constants.frameEnd;

  var c = new Buffer(b.used);
  b.copy(c);

  debug && debug("sending frame: " + c.toJSON());

  this.write(c);

  this._outboundHeartbeatTimerReset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype._startHandshake"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>_startHandshake ()](#apidoc.element.amqp.Connection.prototype._startHandshake)
- description and source-code
```javascript
_startHandshake = function () {
  debug && debug("Initiating handshake...");
  this.write("AMQP" + String.fromCharCode(0,0,9,1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.addAllListeners"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>addAllListeners ()](#apidoc.element.amqp.Connection.prototype.addAllListeners)
- description and source-code
```javascript
addAllListeners = function () {
  var self = this;
  var connectEvent = this.options.ssl.enabled ? 'secureConnect' : 'connect';


  self.addListener(connectEvent, function() {
    // In the case where this is a reconnection, do not trample on the existing
    // channels.
    // For your reference, channel 0 is the control channel.
    self.channels = self.channels || {0:self};
    self.queues = self.queues || {};
    self.exchanges = self.exchanges || {};

    self.parser = new AMQPParser('0-9-1', 'client');

    self.parser.onMethod = function (channel, method, args) {
      self._onMethod(channel, method, args);
    };

    self.parser.onContent = function (channel, data) {
      debug && debug(channel + " > content " + data.length);
      if (self.channels[channel] && self.channels[channel]._onContent) {
        self.channels[channel]._onContent(channel, data);
      } else {
        debug && debug("unhandled content: " + data);
      }
    };

    self.parser.onContentHeader = function (channel, classInfo, weight, properties, size) {
      debug && debug(channel + " > content header " + JSON.stringify([classInfo.name, weight, properties, size]));
      if (self.channels[channel] && self.channels[channel]._onContentHeader) {
        self.channels[channel]._onContentHeader(channel, classInfo, weight, properties, size);
      } else {
        debug && debug("unhandled content header");
      }
    };

    self.parser.onHeartBeat = function () {
      self.emit("heartbeat");
      debug && debug("heartbeat");
    };

    self.parser.onError = function (e) {
      self.emit("error", e);
      self.emit("close");
    };

    // Remove readyEmitted flag so we can detect an auth error.
    self.readyEmitted = false;
  });

  self.addListener('data', function (data) {
    if(self.parser != null){
      try {
        self.parser.execute(data);
      } catch (exception) {
        self.emit('error', exception);
        return;
      }
    }
    self._inboundHeartbeatTimerReset();
  });

  var backoffTime = null;
  self.addListener('error', function backoff(e) {
    if (self._inboundHeartbeatTimer !== null) {
      clearTimeout(self._inboundHeartbeatTimer);
      self._inboundHeartbeatTimer = null;
    }
    if (self._outboundHeartbeatTimer !== null) {
      clearTimeout(self._outboundHeartbeatTimer);
      self._outboundHeartbeatTimer = null;
    }

    if (!self.connectionAttemptScheduled) {
      // Set to true, as we are presently in the process of scheduling one.
      self.connectionAttemptScheduled = true;

      // Kill the socket, if it hasn't been killed already.
      self.socket.end();

      // Reset parser state
      self.parser = null;

      // In order for our reconnection to be seamless, we have to notify the
      // channels that they are no longer connected so that nobody attempts
      // to send messages which would be doomed to fail.
      for (var channel in self.channels) {
        if (channel !== '0') {
          self.channels[channel].state = 'closed';
        }
      }
      // Queues are channels (so we have already marked them as closed), but
      // queues have special needs, since the subscriptions will no longer
      // be known to the server when we reconnect.  Mark the subscriptions as
      // closed so that we can resubscribe them once we are reconnected.
      for (var queue in self.queues) {
        for (var index in self.queues[queue].consumerTagOptions) {
          self.queues[queue].consumerTagOptions[index]['state'] = 'closed';
        }
      }

      // Begin reconnection attempts
      if (self.implOptions.reconnect) {
        // Don't thrash, use a backoff strategy.
        if (backoffTime === null) {
          // This is the first time we've failed since a successful connection,
          // so use the configured backoff time without any modification.
          backoffTime = self.implOptions.reconnectBackoffTime;
        } else if (self.implOptions.reconnectBackoffStrategy === 'exponential') {
          // If you've configured exponential backoff, we'll double the
          // backoff time each ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.connect"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>connect ()](#apidoc.element.amqp.Connection.prototype.connect)
- description and source-code
```javascript
connect = function () {
  // If this is our first connection, add listeners.
  if (!this.socket) this.addAllListeners();

  this._createSocket();
  this._startHandshake();
}
```
- example usage
```shell
...
  });
});
'''

## Connection

'new amqp.Connection()' Instantiates a new connection. Use
'connection.connect()' to connect to a server.

'amqp.createConnection()' returns an instance of 'amqp.Connection', which contains
an instance of 'net.Socket' at its 'socket' property. All events and methods which work on
'net.Socket' can also be used on an 'amqp.Connection' instance. (e.g., the
events ''connect'' and ''close''.)

### Connection options and URL
...
```

#### <a name="apidoc.element.amqp.Connection.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>disconnect ()](#apidoc.element.amqp.Connection.prototype.disconnect)
- description and source-code
```javascript
disconnect = function () {
  debug && debug("Sending disconnect request to server");
  this._sendMethod(0, methods.connectionClose, {
    'replyText': 'client disconnect',
    'replyCode': 200,
    'classId': 0,
    'methodId': 0
  });
}
```
- example usage
```shell
...
## Table of Contents

- [Installation](#installation)
- [Synopsis](#synopsis)
- [Connection](#connection)
- [Connection options and URL](#connection-options-and-url)
- [connection.publish(routingKey, body, options, callback)](#connectionpublishroutingkey-body-options-callback)
- [connection.disconnect()](#connectiondisconnect)
- [Queue](#queue)
- [connection.queue(name[, options][, openCallback])](#connectionqueuename-options-opencallback)
- [queue.subscribe([options,] listener)](#queuesubscribeoptions-listener)
- [queue.subscribeRaw([options,] listener)](#queuesubscriberawoptions-listener)
- [queue.unsubscribe(consumerTag)](#queueunsubscribeconsumertag)
- [queue.shift([reject[, requeue]])](#queueshiftreject-requeue)
- [queue.bind([exchange,] routing)](#queuebindexchange-routing-callback)
...
```

#### <a name="apidoc.element.amqp.Connection.prototype.end"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>end ()](#apidoc.element.amqp.Connection.prototype.end)
- description and source-code
```javascript
end = function () {
  if (this.socket) {
    this.socket.end();
  }

  this.options.heartbeat = false;

  if (this._inboundHeartbeatTimer !== null) {
    clearTimeout(this._inboundHeartbeatTimer);
    this._inboundHeartbeatTimer = null;
  }

  if (this._outboundHeartbeatTimer !== null) {
    clearTimeout(this._outboundHeartbeatTimer);
    this._outboundHeartbeatTimer = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.exchange"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>exchange (name, options, openCallback)](#apidoc.element.amqp.Connection.prototype.exchange)
- description and source-code
```javascript
exchange = function (name, options, openCallback) {
  if (name === undefined) name = this.implOptions.defaultExchangeName;

  if (!options) options = {};
  if (name !== '' && options.type === undefined) options.type = 'topic';

  try{
    var channel = this.generateChannelId();
  }catch(exception){
    this.emit("error", exception);
    return;
  }
  var exchange = new Exchange(this, channel, name, options, openCallback);
  this.channels[channel] = exchange;
  this.exchanges[name] = exchange;
  return exchange;
}
```
- example usage
```shell
...
- [queue.shift([reject[, requeue]])](#queueshiftreject-requeue)
- [queue.bind([exchange,] routing)](#queuebindexchange-routing-callback)
- [queue.unbind([exchange,] routing)](#queueunbindexchange-routing)
- [queue.bind_headers([exchange,] routing)](#queuebind_headersexchange-routing)
- [queue.destroy(options)](#queuedestroyoptions)
- [Exchange](#exchange)
- [exchange.on('open', callback)](#exchangeonopen-callback)
- [connection.exchange()](#connectionexchange)
- [connection.exchange(name, options={}, openCallback)](#connectionexchangename-options-opencallback)
- [exchange.publish(routingKey, message, options, callback)](#exchangepublishroutingkey-message-options-callback)
- [exchange.destroy(ifUnused = true)](#exchangedestroyifunused--true)
- [exchange.bind(srcExchange, routingKey [, callback])](#exchangebindsrcexchange-routingkey--callback)
- [exchange.unbind(srcExchange, routingKey [, callback])](#exchangeunbindsrcexchange-routingkey--callback)
- [exchange.bind_headers(exchange, routing [, bindCallback])](#exchangebind_headersexchange-routing--bindcallback)
...
```

#### <a name="apidoc.element.amqp.Connection.prototype.exchangeClosed"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>exchangeClosed (name)](#apidoc.element.amqp.Connection.prototype.exchangeClosed)
- description and source-code
```javascript
exchangeClosed = function (name) {
  if (this.exchanges[name]) delete this.exchanges[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.generateChannelId"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>generateChannelId ()](#apidoc.element.amqp.Connection.prototype.generateChannelId)
- description and source-code
```javascript
generateChannelId = function () {
  // start from the last used slot id
  var channelId = this.channelCounter;
  while(true){
    // use values in range of 1..65535
    channelId = channelId % channelMax + 1;
    if(!this.channels[channelId]){
      break;
    }
    // after a full loop throw an Error
    if(channelId == this.channelCounter){
      throw new Error("No valid Channel Id values available");
    }
  }
  this.channelCounter = channelId;
  return this.channelCounter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.heartbeat"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>heartbeat ()](#apidoc.element.amqp.Connection.prototype.heartbeat)
- description and source-code
```javascript
heartbeat = function () {
  if(this.socket.writable) this.write(new Buffer([8,0,0,0,0,0,0,206]));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.publish"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>publish (routingKey, body, options, callback)](#apidoc.element.amqp.Connection.prototype.publish)
- description and source-code
```javascript
publish = function (routingKey, body, options, callback) {
  if (!this._defaultExchange) {
    this._defaultExchange = this.exchange();
  }

  var exchange = this._defaultExchange;
  if (exchange.state === 'open') {
    exchange.publish(routingKey, body, options, callback);
  } else {
    exchange.once('open', function() {
      exchange.publish(routingKey, body, options, callback);
    });
  }
}
```
- example usage
```shell
...

## Table of Contents

- [Installation](#installation)
- [Synopsis](#synopsis)
- [Connection](#connection)
- [Connection options and URL](#connection-options-and-url)
- [connection.publish(routingKey, body, options, callback)](#connectionpublishroutingkey-body-options-callback)
- [connection.disconnect()](#connectiondisconnect)
- [Queue](#queue)
- [connection.queue(name[, options][, openCallback])](#connectionqueuename-options-opencallback)
- [queue.subscribe([options,] listener)](#queuesubscribeoptions-listener)
- [queue.subscribeRaw([options,] listener)](#queuesubscriberawoptions-listener)
- [queue.unsubscribe(consumerTag)](#queueunsubscribeconsumertag)
- [queue.shift([reject[, requeue]])](#queueshiftreject-requeue)
...
```

#### <a name="apidoc.element.amqp.Connection.prototype.queue"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>queue (name)](#apidoc.element.amqp.Connection.prototype.queue)
- description and source-code
```javascript
queue = function (name) {
  var options, callback;
  if (typeof arguments[1] == 'object') {
    options = arguments[1];
    callback = arguments[2];
  } else {
    callback = arguments[1];
  }

  try{
    var channel = this.generateChannelId();
  }catch(exception){
    this.emit("error", exception);
    return;
  }

  var q = new Queue(this, channel, name, options, callback);
  this.channels[channel] = q;
  return q;
}
```
- example usage
```shell
...
- [Installation](#installation)
- [Synopsis](#synopsis)
- [Connection](#connection)
- [Connection options and URL](#connection-options-and-url)
- [connection.publish(routingKey, body, options, callback)](#connectionpublishroutingkey-body-options-callback)
- [connection.disconnect()](#connectiondisconnect)
- [Queue](#queue)
- [connection.queue(name[, options][, openCallback])](#connectionqueuename-options-opencallback)
- [queue.subscribe([options,] listener)](#queuesubscribeoptions-listener)
- [queue.subscribeRaw([options,] listener)](#queuesubscriberawoptions-listener)
- [queue.unsubscribe(consumerTag)](#queueunsubscribeconsumertag)
- [queue.shift([reject[, requeue]])](#queueshiftreject-requeue)
- [queue.bind([exchange,] routing)](#queuebindexchange-routing-callback)
- [queue.unbind([exchange,] routing)](#queueunbindexchange-routing)
- [queue.bind_headers([exchange,] routing)](#queuebind_headersexchange-routing)
...
```

#### <a name="apidoc.element.amqp.Connection.prototype.queueClosed"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>queueClosed (name)](#apidoc.element.amqp.Connection.prototype.queueClosed)
- description and source-code
```javascript
queueClosed = function (name) {
  if (this.queues[name]) delete this.queues[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.reconnect"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>reconnect ()](#apidoc.element.amqp.Connection.prototype.reconnect)
- description and source-code
```javascript
reconnect = function () {
  // Suspend activity on channels
  for (var channel in this.channels) {
    this.channels[channel].state = 'closed';
  }
  debug && debug("Connection lost, reconnecting...");
  // Terminate socket activity
  if (this.socket) this.socket.end();
  this.connect();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.setImplOptions"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>setImplOptions (options)](#apidoc.element.amqp.Connection.prototype.setImplOptions)
- description and source-code
```javascript
setImplOptions = function (options) {
  this.implOptions = _.assignIn({}, defaultImplOptions, options || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.amqp.Connection.prototype.setOptions"></a>[function <span class="apidocSignatureSpan">amqp.Connection.prototype.</span>setOptions (options)](#apidoc.element.amqp.Connection.prototype.setOptions)
- description and source-code
```javascript
setOptions = function (options) {
  var urlo = (options && options.url) ? this._parseURLOptions(options.url) : {};
  var sslo = (options && options.ssl && options.ssl.enabled) ? defaultSslOptions : {};
  this.options = _.assignIn({}, defaultOptions, sslo, urlo, options || {});
  this.options.clientProperties =  _.assignIn({}, defaultClientProperties, (options && options.clientProperties) || {});
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
