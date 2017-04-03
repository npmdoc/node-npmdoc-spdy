# api documentation for  [spdy (v3.4.4)](https://github.com/indutny/node-spdy)  [![npm package](https://img.shields.io/npm/v/npmdoc-spdy.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-spdy) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-spdy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-spdy)
#### Implementation of the SPDY protocol on node.js.

[![NPM](https://nodei.co/npm/spdy.png?downloads=true)](https://www.npmjs.com/package/spdy)

[![apidoc](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-spdy_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-spdy/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fedor Indutny",
        "email": "fedor.indutny@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/indutny/node-spdy/issues",
        "email": "node-spdy+bugs@indutny.com"
    },
    "contributors": [
        {
            "name": "Chris Storm",
            "email": "github@eeecooks.com"
        },
        {
            "name": "François de Metz",
            "email": "francois@2metz.fr"
        },
        {
            "name": "Ilya Grigorik",
            "email": "ilya@igvita.com"
        },
        {
            "name": "Roberto Peon"
        },
        {
            "name": "Tatsuhiro Tsujikawa"
        },
        {
            "name": "Jesse Cravens",
            "email": "jesse.cravens@gmail.com"
        }
    ],
    "dependencies": {
        "debug": "^2.2.0",
        "handle-thing": "^1.2.4",
        "http-deceiver": "^1.2.4",
        "select-hose": "^2.0.0",
        "spdy-transport": "^2.0.15"
    },
    "description": "Implementation of the SPDY protocol on node.js.",
    "devDependencies": {
        "jscs": "^1.13.1",
        "jshint": "^2.8.0",
        "mocha": "^2.2.x"
    },
    "directories": {},
    "dist": {
        "shasum": "e0406407ca90ff01b553eb013505442649f5a819",
        "tarball": "https://registry.npmjs.org/spdy/-/spdy-3.4.4.tgz"
    },
    "engines": [
        "node >= 0.7.0"
    ],
    "gitHead": "52dc157eef87d7d2bb7b39ab25fdcfee45f88dd9",
    "homepage": "https://github.com/indutny/node-spdy",
    "keywords": [
        "spdy"
    ],
    "license": "MIT",
    "main": "./lib/spdy",
    "maintainers": [
        {
            "name": "fedor.indutny",
            "email": "fedor.indutny@gmail.com"
        },
        {
            "name": "indutny",
            "email": "fedor@indutny.com"
        },
        {
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        }
    ],
    "name": "spdy",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/indutny/node-spdy.git"
    },
    "scripts": {
        "test": "jscs lib/**/*.js test/*.js && jshint lib/**/*.js && mocha --reporter=spec test/*-test.js"
    },
    "version": "3.4.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module spdy](#apidoc.module.spdy)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Agent (options)](#apidoc.element.spdy.Agent)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Agent.super_ (options)](#apidoc.element.spdy.Agent.super_)
1.  [function <span class="apidocSignatureSpan">spdy.</span>PlainServer (options, handler)](#apidoc.element.spdy.PlainServer)
1.  [function <span class="apidocSignatureSpan">spdy.</span>PlainServer.super_ (requestListener)](#apidoc.element.spdy.PlainServer.super_)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Server (options, handler)](#apidoc.element.spdy.Server)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Server.super_ (opts, requestListener)](#apidoc.element.spdy.Server.super_)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Socket (parent, options)](#apidoc.element.spdy.Socket)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Socket.super_ (options)](#apidoc.element.spdy.Socket.super_)
1.  [function <span class="apidocSignatureSpan">spdy.</span>agent.PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent)
1.  [function <span class="apidocSignatureSpan">spdy.</span>createAgent (base, options)](#apidoc.element.spdy.createAgent)
1.  [function <span class="apidocSignatureSpan">spdy.</span>createServer (base, options, handler)](#apidoc.element.spdy.createServer)
1.  [function <span class="apidocSignatureSpan">spdy.</span>handle (options, stream, socket)](#apidoc.element.spdy.handle)
1.  [function <span class="apidocSignatureSpan">spdy.</span>handle.super_ (stream, options)](#apidoc.element.spdy.handle.super_)
1.  object <span class="apidocSignatureSpan">spdy.</span>Agent.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Agent.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Agent.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>PlainServer.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>PlainServer.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>PlainServer.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Server.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Server.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Server.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Socket.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>Socket.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>agent
1.  object <span class="apidocSignatureSpan">spdy.</span>agent.PlainAgent.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>handle.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>handle.super_.prototype
1.  object <span class="apidocSignatureSpan">spdy.</span>request
1.  object <span class="apidocSignatureSpan">spdy.</span>response
1.  object <span class="apidocSignatureSpan">spdy.</span>server

#### [module spdy.Agent](#apidoc.module.spdy.Agent)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Agent (options)](#apidoc.element.spdy.Agent.Agent)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.</span>create (options)](#apidoc.element.spdy.Agent.create)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.</span>super_ (options)](#apidoc.element.spdy.Agent.super_)

#### [module spdy.Agent.prototype](#apidoc.module.spdy.Agent.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_connect (options, callback)](#apidoc.element.spdy.Agent.prototype._connect)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_createSocket (req, options, callback)](#apidoc.element.spdy.Agent.prototype._createSocket)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_createStream (req, handle)](#apidoc.element.spdy.Agent.prototype._createStream)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_getCreateSocket ()](#apidoc.element.spdy.Agent.prototype._getCreateSocket)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_init (base, options)](#apidoc.element.spdy.Agent.prototype._init)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>close (callback)](#apidoc.element.spdy.Agent.prototype.close)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>createSocket (req, options, callback)](#apidoc.element.spdy.Agent.prototype.createSocket)

#### [module spdy.Agent.super_](#apidoc.module.spdy.Agent.super_)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.</span>super_ (options)](#apidoc.element.spdy.Agent.super_.super_)

#### [module spdy.Agent.super_.prototype](#apidoc.module.spdy.Agent.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_cacheSession (key, session)](#apidoc.element.spdy.Agent.super_.prototype._cacheSession)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_evictSession (key)](#apidoc.element.spdy.Agent.super_.prototype._evictSession)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_getSession (key)](#apidoc.element.spdy.Agent.super_.prototype._getSession)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>createConnection (port, host, options)](#apidoc.element.spdy.Agent.super_.prototype.createConnection)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>getName (options)](#apidoc.element.spdy.Agent.super_.prototype.getName)

#### [module spdy.Agent.super_.super_.prototype](#apidoc.module.spdy.Agent.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>addRequest (req, options)](#apidoc.element.spdy.Agent.super_.super_.prototype.addRequest)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>createConnection ()](#apidoc.element.spdy.Agent.super_.super_.prototype.createConnection)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>createSocket (req, options, cb)](#apidoc.element.spdy.Agent.super_.super_.prototype.createSocket)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>destroy ()](#apidoc.element.spdy.Agent.super_.super_.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>getName (options)](#apidoc.element.spdy.Agent.super_.super_.prototype.getName)
1.  [function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>removeSocket (s, options)](#apidoc.element.spdy.Agent.super_.super_.prototype.removeSocket)

#### [module spdy.PlainServer](#apidoc.module.spdy.PlainServer)
1.  [function <span class="apidocSignatureSpan">spdy.</span>PlainServer (options, handler)](#apidoc.element.spdy.PlainServer.PlainServer)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.</span>create (options, handler)](#apidoc.element.spdy.PlainServer.create)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.</span>super_ (requestListener)](#apidoc.element.spdy.PlainServer.super_)

#### [module spdy.PlainServer.prototype](#apidoc.module.spdy.PlainServer.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_handleConnection (socket, protocol)](#apidoc.element.spdy.PlainServer.prototype._handleConnection)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_init (base, options, handler)](#apidoc.element.spdy.PlainServer.prototype._init)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_invokeDefault (socket)](#apidoc.element.spdy.PlainServer.prototype._invokeDefault)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onConnection (socket)](#apidoc.element.spdy.PlainServer.prototype._onConnection)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onPlainConnection (socket)](#apidoc.element.spdy.PlainServer.prototype._onPlainConnection)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onStream (stream)](#apidoc.element.spdy.PlainServer.prototype._onStream)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>emit (event, req, res)](#apidoc.element.spdy.PlainServer.prototype.emit)

#### [module spdy.PlainServer.super_](#apidoc.module.spdy.PlainServer.super_)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.</span>super_ (options, connectionListener)](#apidoc.element.spdy.PlainServer.super_.super_)

#### [module spdy.PlainServer.super_.prototype](#apidoc.module.spdy.PlainServer.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.PlainServer.super_.prototype.setTimeout)

#### [module spdy.PlainServer.super_.super_.prototype](#apidoc.module.spdy.PlainServer.super_.super_.prototype)
1.  boolean <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>listening
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_emitCloseIfDrained ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype._emitCloseIfDrained)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_listen2 (address, port, addressType, backlog, fd)](#apidoc.element.spdy.PlainServer.super_.super_.prototype._listen2)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_setupSlave (socketList)](#apidoc.element.spdy.PlainServer.super_.super_.prototype._setupSlave)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>address ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.address)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>close (cb)](#apidoc.element.spdy.PlainServer.super_.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>getConnections (cb)](#apidoc.element.spdy.PlainServer.super_.super_.prototype.getConnections)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>listen ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.listen)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>listenFD ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.listenFD)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>ref ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.ref)
1.  [function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>unref ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.unref)

#### [module spdy.Server](#apidoc.module.spdy.Server)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Server (options, handler)](#apidoc.element.spdy.Server.Server)
1.  [function <span class="apidocSignatureSpan">spdy.Server.</span>create (options, handler)](#apidoc.element.spdy.Server.create)
1.  [function <span class="apidocSignatureSpan">spdy.Server.</span>super_ (opts, requestListener)](#apidoc.element.spdy.Server.super_)

#### [module spdy.Server.prototype](#apidoc.module.spdy.Server.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_handleConnection (socket, protocol)](#apidoc.element.spdy.Server.prototype._handleConnection)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_init (base, options, handler)](#apidoc.element.spdy.Server.prototype._init)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_invokeDefault (socket)](#apidoc.element.spdy.Server.prototype._invokeDefault)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onConnection (socket)](#apidoc.element.spdy.Server.prototype._onConnection)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onPlainConnection (socket)](#apidoc.element.spdy.Server.prototype._onPlainConnection)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onStream (stream)](#apidoc.element.spdy.Server.prototype._onStream)
1.  [function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>emit (event, req, res)](#apidoc.element.spdy.Server.prototype.emit)

#### [module spdy.Server.super_](#apidoc.module.spdy.Server.super_)
1.  [function <span class="apidocSignatureSpan">spdy.Server.</span>super_ (options, listener)](#apidoc.element.spdy.Server.super_.super_)

#### [module spdy.Server.super_.prototype](#apidoc.module.spdy.Server.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.Server.super_.prototype.setTimeout)

#### [module spdy.Server.super_.super_.prototype](#apidoc.module.spdy.Server.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>_getServerData ()](#apidoc.element.spdy.Server.super_.super_.prototype._getServerData)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>_setServerData (data)](#apidoc.element.spdy.Server.super_.super_.prototype._setServerData)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>addContext (servername, context)](#apidoc.element.spdy.Server.super_.super_.prototype.addContext)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>getTicketKeys (keys)](#apidoc.element.spdy.Server.super_.super_.prototype.getTicketKeys)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>setOptions (options)](#apidoc.element.spdy.Server.super_.super_.prototype.setOptions)
1.  [function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>setTicketKeys (keys)](#apidoc.element.spdy.Server.super_.super_.prototype.setTicketKeys)

#### [module spdy.Socket](#apidoc.module.spdy.Socket)
1.  [function <span class="apidocSignatureSpan">spdy.</span>Socket (parent, options)](#apidoc.element.spdy.Socket.Socket)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.</span>super_ (options)](#apidoc.element.spdy.Socket.super_)

#### [module spdy.Socket.prototype](#apidoc.module.spdy.Socket.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getCipher ()](#apidoc.element.spdy.Socket.prototype.getCipher)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getEphemeralKeyInfo ()](#apidoc.element.spdy.Socket.prototype.getEphemeralKeyInfo)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getPeerCertificate ()](#apidoc.element.spdy.Socket.prototype.getPeerCertificate)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getSession ()](#apidoc.element.spdy.Socket.prototype.getSession)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getTLSTicket ()](#apidoc.element.spdy.Socket.prototype.getTLSTicket)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>isSessionReused ()](#apidoc.element.spdy.Socket.prototype.isSessionReused)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>renegotiate ()](#apidoc.element.spdy.Socket.prototype.renegotiate)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setMaxSendFragment ()](#apidoc.element.spdy.Socket.prototype.setMaxSendFragment)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setServername ()](#apidoc.element.spdy.Socket.prototype.setServername)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setSession ()](#apidoc.element.spdy.Socket.prototype.setSession)

#### [module spdy.Socket.super_](#apidoc.module.spdy.Socket.super_)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.</span>super_ (options)](#apidoc.element.spdy.Socket.super_.super_)

#### [module spdy.Socket.super_.prototype](#apidoc.module.spdy.Socket.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_destroy (exception, cb)](#apidoc.element.spdy.Socket.super_.prototype._destroy)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_getpeername ()](#apidoc.element.spdy.Socket.super_.prototype._getpeername)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_getsockname ()](#apidoc.element.spdy.Socket.super_.prototype._getsockname)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_onTimeout ()](#apidoc.element.spdy.Socket.super_.prototype._onTimeout)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_read (n)](#apidoc.element.spdy.Socket.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_unrefTimer ()](#apidoc.element.spdy.Socket.super_.prototype._unrefTimer)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_write (data, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_writeGeneric (writev, data, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype._writeGeneric)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_writev (chunks, cb)](#apidoc.element.spdy.Socket.super_.prototype._writev)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>address ()](#apidoc.element.spdy.Socket.super_.prototype.address)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>connect (options, cb)](#apidoc.element.spdy.Socket.super_.prototype.connect)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>destroy (exception)](#apidoc.element.spdy.Socket.super_.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>destroySoon ()](#apidoc.element.spdy.Socket.super_.prototype.destroySoon)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>end (data, encoding)](#apidoc.element.spdy.Socket.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>listen ()](#apidoc.element.spdy.Socket.super_.prototype.listen)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>read (n)](#apidoc.element.spdy.Socket.super_.prototype.read)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>ref ()](#apidoc.element.spdy.Socket.super_.prototype.ref)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setKeepAlive (setting, msecs)](#apidoc.element.spdy.Socket.super_.prototype.setKeepAlive)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setNoDelay (enable)](#apidoc.element.spdy.Socket.super_.prototype.setNoDelay)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.Socket.super_.prototype.setTimeout)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>unref ()](#apidoc.element.spdy.Socket.super_.prototype.unref)
1.  [function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype.write)

#### [module spdy.agent](#apidoc.module.spdy.agent)
1.  [function <span class="apidocSignatureSpan">spdy.agent.</span>Agent (options)](#apidoc.element.spdy.agent.Agent)
1.  [function <span class="apidocSignatureSpan">spdy.agent.</span>PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent)
1.  [function <span class="apidocSignatureSpan">spdy.agent.</span>create (base, options)](#apidoc.element.spdy.agent.create)

#### [module spdy.agent.PlainAgent](#apidoc.module.spdy.agent.PlainAgent)
1.  [function <span class="apidocSignatureSpan">spdy.agent.</span>PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent.PlainAgent)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.</span>create (options)](#apidoc.element.spdy.agent.PlainAgent.create)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.</span>super_ (options)](#apidoc.element.spdy.agent.PlainAgent.super_)

#### [module spdy.agent.PlainAgent.prototype](#apidoc.module.spdy.agent.PlainAgent.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_connect (options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype._connect)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_createSocket (req, options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype._createSocket)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_createStream (req, handle)](#apidoc.element.spdy.agent.PlainAgent.prototype._createStream)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_getCreateSocket ()](#apidoc.element.spdy.agent.PlainAgent.prototype._getCreateSocket)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_init (base, options)](#apidoc.element.spdy.agent.PlainAgent.prototype._init)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>close (callback)](#apidoc.element.spdy.agent.PlainAgent.prototype.close)
1.  [function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>createSocket (req, options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype.createSocket)

#### [module spdy.handle](#apidoc.module.spdy.handle)
1.  [function <span class="apidocSignatureSpan">spdy.</span>handle (options, stream, socket)](#apidoc.element.spdy.handle.handle)
1.  [function <span class="apidocSignatureSpan">spdy.handle.</span>create (options, stream, socket)](#apidoc.element.spdy.handle.create)
1.  [function <span class="apidocSignatureSpan">spdy.handle.</span>super_ (stream, options)](#apidoc.element.spdy.handle.super_)

#### [module spdy.handle.prototype](#apidoc.module.spdy.handle.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_closeCallback (callback)](#apidoc.element.spdy.handle.prototype._closeCallback)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_getPeerName ()](#apidoc.element.spdy.handle.prototype._getPeerName)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_transformHeaders (kind, headers)](#apidoc.element.spdy.handle.prototype._transformHeaders)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignClientRequest (req)](#apidoc.element.spdy.handle.prototype.assignClientRequest)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignRequest (req)](#apidoc.element.spdy.handle.prototype.assignRequest)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignResponse (res)](#apidoc.element.spdy.handle.prototype.assignResponse)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignSocket (socket, options)](#apidoc.element.spdy.handle.prototype.assignSocket)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>emitRequest ()](#apidoc.element.spdy.handle.prototype.emitRequest)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>emitResponse (status, headers)](#apidoc.element.spdy.handle.prototype.emitResponse)
1.  [function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>getStream (callback)](#apidoc.element.spdy.handle.prototype.getStream)

#### [module spdy.handle.super_](#apidoc.module.spdy.handle.super_)
1.  [function <span class="apidocSignatureSpan">spdy.handle.</span>super_ ()](#apidoc.element.spdy.handle.super_.super_)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.</span>create (stream, options)](#apidoc.element.spdy.handle.super_.create)
1.  string <span class="apidocSignatureSpan">spdy.handle.super_.</span>mode

#### [module spdy.handle.super_.prototype](#apidoc.module.spdy.handle.super_.prototype)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_close ()](#apidoc.element.spdy.handle.super_.prototype._close)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_flow ()](#apidoc.element.spdy.handle.super_.prototype._flow)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_pendingList ()](#apidoc.element.spdy.handle.super_.prototype._pendingList)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_queueReq (type, req)](#apidoc.element.spdy.handle.super_.prototype._queueReq)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_shutdown (wrap)](#apidoc.element.spdy.handle.super_.prototype._shutdown)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_writeEnc (wrap, req, data, enc)](#apidoc.element.spdy.handle.super_.prototype._writeEnc)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>close (callback)](#apidoc.element.spdy.handle.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>getpeername (out)](#apidoc.element.spdy.handle.super_.prototype.getpeername)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>getsockname ()](#apidoc.element.spdy.handle.super_.prototype.getsockname)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>readStart ()](#apidoc.element.spdy.handle.super_.prototype.readStart)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>readStop ()](#apidoc.element.spdy.handle.super_.prototype.readStop)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>setStream (stream)](#apidoc.element.spdy.handle.super_.prototype.setStream)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>shutdown (req)](#apidoc.element.spdy.handle.super_.prototype.shutdown)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeAsciiString (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeAsciiString)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeBinaryString (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeBinaryString)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeBuffer (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeBuffer)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeEnc (req, data, enc)](#apidoc.element.spdy.handle.super_.prototype.writeEnc)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeLatin1String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeLatin1String)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeUcs2String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeUcs2String)
1.  [function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeUtf8String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeUtf8String)

#### [module spdy.request](#apidoc.module.spdy.request)
1.  [function <span class="apidocSignatureSpan">spdy.request.</span>onNewListener (type)](#apidoc.element.spdy.request.onNewListener)

#### [module spdy.response](#apidoc.module.spdy.response)
1.  [function <span class="apidocSignatureSpan">spdy.response.</span>end (data, encoding, callback)](#apidoc.element.spdy.response.end)
1.  [function <span class="apidocSignatureSpan">spdy.response.</span>push (path, headers, callback)](#apidoc.element.spdy.response.push)
1.  [function <span class="apidocSignatureSpan">spdy.response.</span>writeContinue (callback)](#apidoc.element.spdy.response.writeContinue)
1.  [function <span class="apidocSignatureSpan">spdy.response.</span>writeHead (statusCode, reason, obj)](#apidoc.element.spdy.response.writeHead)

#### [module spdy.server](#apidoc.module.spdy.server)
1.  [function <span class="apidocSignatureSpan">spdy.server.</span>PlainServer (options, handler)](#apidoc.element.spdy.server.PlainServer)
1.  [function <span class="apidocSignatureSpan">spdy.server.</span>Server (options, handler)](#apidoc.element.spdy.server.Server)
1.  [function <span class="apidocSignatureSpan">spdy.server.</span>create (base, options, handler)](#apidoc.element.spdy.server.create)



# <a name="apidoc.module.spdy"></a>[module spdy](#apidoc.module.spdy)

#### <a name="apidoc.element.spdy.Agent"></a>[function <span class="apidocSignatureSpan">spdy.</span>Agent (options)](#apidoc.element.spdy.Agent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_"></a>[function <span class="apidocSignatureSpan">spdy.</span>Agent.super_ (options)](#apidoc.element.spdy.Agent.super_)
- description and source-code
```javascript
function Agent(options) {
  http.Agent.call(this, options);
  this.defaultPort = 443;
  this.protocol = 'https:';
  this.maxCachedSessions = this.options.maxCachedSessions;
  if (this.maxCachedSessions === undefined)
    this.maxCachedSessions = 100;

  this._sessionCache = {
    map: {},
    list: []
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer"></a>[function <span class="apidocSignatureSpan">spdy.</span>PlainServer (options, handler)](#apidoc.element.spdy.PlainServer)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_"></a>[function <span class="apidocSignatureSpan">spdy.</span>PlainServer.super_ (requestListener)](#apidoc.element.spdy.PlainServer.super_)
- description and source-code
```javascript
function Server(requestListener) {
  if (!(this instanceof Server)) return new Server(requestListener);
  net.Server.call(this, { allowHalfOpen: true });

  if (requestListener) {
    this.addListener('request', requestListener);
  }

<span class="apidocCodeCommentSpan">  /* eslint-disable max-len */
</span>  // Similar option to this. Too lazy to write my own docs.
  // http://www.squid-cache.org/Doc/config/half_closed_clients/
  // http://wiki.squid-cache.org/SquidFaq/InnerWorkings#What_is_a_half-closed_filedescriptor.3F
  /* eslint-enable max-len */
  this.httpAllowHalfOpen = false;

  this.addListener('connection', connectionListener);

  this.timeout = 2 * 60 * 1000;

  this._pendingResponseData = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server"></a>[function <span class="apidocSignatureSpan">spdy.</span>Server (options, handler)](#apidoc.element.spdy.Server)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_"></a>[function <span class="apidocSignatureSpan">spdy.</span>Server.super_ (opts, requestListener)](#apidoc.element.spdy.Server.super_)
- description and source-code
```javascript
function Server(opts, requestListener) {
  if (!(this instanceof Server)) return new Server(opts, requestListener);

  if (process.features.tls_npn && !opts.NPNProtocols) {
    opts.NPNProtocols = ['http/1.1', 'http/1.0'];
  }

  if (process.features.tls_alpn && !opts.ALPNProtocols) {
    // http/1.0 is not defined as Protocol IDs in IANA
    // http://www.iana.org/assignments/tls-extensiontype-values
    //       /tls-extensiontype-values.xhtml#alpn-protocol-ids
    opts.ALPNProtocols = ['http/1.1'];
  }

  tls.Server.call(this, opts, http._connectionListener);

  this.httpAllowHalfOpen = false;

  if (requestListener) {
    this.addListener('request', requestListener);
  }

  this.addListener('tlsClientError', function(err, conn) {
    if (!this.emit('clientError', err, conn))
      conn.destroy(err);
  });

  this.timeout = 2 * 60 * 1000;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket"></a>[function <span class="apidocSignatureSpan">spdy.</span>Socket (parent, options)](#apidoc.element.spdy.Socket)
- description and source-code
```javascript
function Socket(parent, options) {
  net.Socket.call(this, options);

  var state = {};

  this._spdyState = state;

  state.parent = parent;

  this.servername = parent.servername;
  this.npnProtocol = parent.npnProtocol;
  this.alpnProtocol = parent.alpnProtocol;
  this.authorized = parent.authorized;
  this.authorizationError = parent.authorizationError;
  this.encrypted = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_"></a>[function <span class="apidocSignatureSpan">spdy.</span>Socket.super_ (options)](#apidoc.element.spdy.Socket.super_)
- description and source-code
```javascript
function Socket(options) {
  if (!(this instanceof Socket)) return new Socket(options);

  this.connecting = false;
  this._hadError = false;
  this._handle = null;
  this._parent = null;
  this._host = null;

  if (typeof options === 'number')
    options = { fd: options }; // Legacy interface.
  else if (options === undefined)
    options = {};

  stream.Duplex.call(this, options);

  if (options.handle) {
    this._handle = options.handle; // private
  } else if (options.fd !== undefined) {
    this._handle = createHandle(options.fd);
    this._handle.open(options.fd);
    // options.fd can be string (since it user-defined),
    // so changing this to === would be semver-major
    // See: https://github.com/nodejs/node/pull/11513
    if ((options.fd == 1 || options.fd == 2) &&
        (this._handle instanceof Pipe) &&
        process.platform === 'win32') {
      // Make stdout and stderr blocking on Windows
      var err = this._handle.setBlocking(true);
      if (err)
        throw errnoException(err, 'setBlocking');
    }
    this.readable = options.readable !== false;
    this.writable = options.writable !== false;
  } else {
    // these will be set once there is a connection
    this.readable = this.writable = false;
  }

  // shut down the socket when we're finished with it.
  this.on('finish', onSocketFinish);
  this.on('_socketEnd', onSocketEnd);

  initSocketHandle(this);

  this._pendingData = null;
  this._pendingEncoding = '';

  // handle strings directly
  this._writableState.decodeStrings = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  // if we have a handle, then start the flow of data into the
  // buffer.  if not, then this will happen when we connect
  if (this._handle && options.readable !== false) {
    if (options.pauseOnCreate) {
      // stop the handle from reading and pause the stream
      this._handle.reading = false;
      this._handle.readStop();
      this._readableState.flowing = false;
    } else {
      this.read(0);
    }
  }

  // Reserve properties
  this.server = null;
  this._server = null;

  // Used after '.destroy()'
  this[BYTES_READ] = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent"></a>[function <span class="apidocSignatureSpan">spdy.</span>agent.PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.createAgent"></a>[function <span class="apidocSignatureSpan">spdy.</span>createAgent (base, options)](#apidoc.element.spdy.createAgent)
- description and source-code
```javascript
function create(base, options) {
  if (typeof base === 'object') {
    options = base;
    base = null;
  }

  if (base)
    return instantiate(base).create(options);

  if (options.spdy && options.spdy.plain)
    return exports.PlainAgent.create(options);
  else
    return exports.Agent.create(options);
}
```
- example usage
```shell
...
'''

Client:
'''javascript
var spdy = require('spdy');
var http = require('http');

var agent = spdy.createAgent({
host: 'www.google.com',
port: 443,

// Optional SPDY options
spdy: {
  plain: false or true,
  ssl: false or true,
...
```

#### <a name="apidoc.element.spdy.createServer"></a>[function <span class="apidocSignatureSpan">spdy.</span>createServer (base, options, handler)](#apidoc.element.spdy.createServer)
- description and source-code
```javascript
function create(base, options, handler) {
  if (typeof base === 'object') {
    handler = options;
    options = base;
    base = null;
  }

  if (base)
    return instantiate(base).create(options, handler);

  if (options.spdy && options.spdy.plain)
    return exports.PlainServer.create(options, handler);
  else
    return exports.Server.create(options, handler);
}
```
- example usage
```shell
...

      // **optional** if true - server will send 3.1 frames on 3.0 *plain* spdy
      autoSpdy31: false
    }
  }
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''
...
```

#### <a name="apidoc.element.spdy.handle"></a>[function <span class="apidocSignatureSpan">spdy.</span>handle (options, stream, socket)](#apidoc.element.spdy.handle)
- description and source-code
```javascript
function Handle(options, stream, socket) {
  var state = {};
  this._spdyState = state;

  state.options = options || {};

  state.stream = stream;
  state.socket = null;
  state.rawSocket = socket || stream.connection.socket;
  state.deceiver = null;
  state.ending = false;

  var self = this;
  thing.call(this, stream, {
    getPeerName: function() {
      return self._getPeerName();
    },
    close: function(callback) {
      return self._closeCallback(callback);
    }
  });

  if (!state.stream) {
    this.on('stream', function(stream) {
      state.stream = stream;
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_"></a>[function <span class="apidocSignatureSpan">spdy.</span>handle.super_ (stream, options)](#apidoc.element.spdy.handle.super_)
- description and source-code
```javascript
function Handle(stream, options) {
  EventEmitter.call(this);

  this._stream = stream;
  this._flowing = false;
  this._reading = false;
  this._options = options || {};

  this.onread = null;

  // Pending requests
  this.pending = new Queue();

  // Start handle once 'onread' is set
  if (mode === 'rusty') {
    var self = this;
    Object.defineProperty(this, 'onread', {
      set: function(value) {
        Object.defineProperty(self, 'onread', {
          value: value
        });
        process.nextTick(function() {
          self.readStart();
        });
      }
    });
  }

  // NOTE: v0.8 has some odd .pause()/.resume() semantics in http.js
  if (mode === 'rusty')
    this.writeQueueSize = 0;
  else if (mode !== 'modern')
    this.writeQueueSize = 1;

  if (mode === 'rusty') {
    if (this._stream)
      this._rustyInit();
    else
      this.once('stream', this._rustyInit);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Agent"></a>[module spdy.Agent](#apidoc.module.spdy.Agent)

#### <a name="apidoc.element.spdy.Agent.Agent"></a>[function <span class="apidocSignatureSpan">spdy.</span>Agent (options)](#apidoc.element.spdy.Agent.Agent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.create"></a>[function <span class="apidocSignatureSpan">spdy.Agent.</span>create (options)](#apidoc.element.spdy.Agent.create)
- description and source-code
```javascript
function create(options) {
  return new Agent(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_"></a>[function <span class="apidocSignatureSpan">spdy.Agent.</span>super_ (options)](#apidoc.element.spdy.Agent.super_)
- description and source-code
```javascript
function Agent(options) {
  http.Agent.call(this, options);
  this.defaultPort = 443;
  this.protocol = 'https:';
  this.maxCachedSessions = this.options.maxCachedSessions;
  if (this.maxCachedSessions === undefined)
    this.maxCachedSessions = 100;

  this._sessionCache = {
    map: {},
    list: []
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Agent.prototype"></a>[module spdy.Agent.prototype](#apidoc.module.spdy.Agent.prototype)

#### <a name="apidoc.element.spdy.Agent.prototype._connect"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_connect (options, callback)](#apidoc.element.spdy.Agent.prototype._connect)
- description and source-code
```javascript
function _connect(options, callback) {
  var state = this._spdyState;

  var protocols = state.options.protocols || [
    'h2',
    'spdy/3.1', 'spdy/3', 'spdy/2',
    'http/1.1', 'http/1.0'
  ];

  // TODO(indutny): reconnect automatically?
  var socket = this.createConnection(util._extend({
    NPNProtocols: protocols,
    ALPNProtocols: protocols,
    servername: options.servername || options.host
  }, options));
  state.socket = socket;

  socket.setNoDelay(true);

  function onError(err) {
    return callback(err);
  }
  socket.on('error', onError);

  socket.on(state.secure ? 'secureConnect' : 'connect', function() {
    socket.removeListener('error', onError);

    var protocol;
    if (state.secure) {
      protocol = socket.npnProtocol ||
                 socket.alpnProtocol ||
                 state.options.protocol;
    } else {
      protocol = state.options.protocol;
    }

    // HTTP server - kill socket and switch to the fallback mode
    if (!protocol || protocol === 'http/1.1' || protocol === 'http/1.0') {
      debug('activating fallback');
      socket.destroy();
      state.fallback = true;
      return;
    }

    debug('connected protocol=%j', protocol);
    var connection = transport.connection.create(socket, util._extend({
      protocol: /spdy/.test(protocol) ? 'spdy' : 'http2',
      isServer: false
    }, state.options.connection || {}));

    // Set version when we are certain
    if (protocol === 'h2') {
      connection.start(4);
    } else if (protocol === 'spdy/3.1') {
      connection.start(3.1);
    } else if (protocol === 'spdy/3') {
      connection.start(3);
    } else if (protocol === 'spdy/2') {
      connection.start(2);
    } else {
      socket.destroy();
      callback(new Error('Unexpected protocol: ' + protocol));
      return;
    }

    if (state.options['x-forwarded-for'] !== undefined)
      connection.sendXForwardedFor(state.options['x-forwarded-for']);

    callback(null, connection);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.prototype._createSocket"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_createSocket (req, options, callback)](#apidoc.element.spdy.Agent.prototype._createSocket)
- description and source-code
```javascript
function _createSocket(req, options, callback) {
  var state = this._spdyState;
  if (state.fallback)
    return state.createSocket(req, options);

  var handle = spdy.handle.create(null, null, state.socket);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(state.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);
  handle.assignClientRequest(req);

  // Create stream only once 'req.end()' is called
  var self = this;
  handle.once('needStream', function() {
    if (state.connection === null) {
      self.once('_connect', function() {
        handle.setStream(self._createStream(req, handle));
      });
    } else {
      handle.setStream(self._createStream(req, handle));
    }
  });

  // Yes, it is in reverse
  req.on('response', function(res) {
    handle.assignRequest(res);
  });
  handle.assignResponse(req);

  // Handle PUSH
  req.addListener('newListener', spdy.request.onNewListener);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  if (callback)
    return callback(null, socket);

  return socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.prototype._createStream"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_createStream (req, handle)](#apidoc.element.spdy.Agent.prototype._createStream)
- description and source-code
```javascript
function _createStream(req, handle) {
  var state = this._spdyState;

  var self = this;
  return state.connection.reserveStream({
    method: req.method,
    path: req.path,
    headers: req._headers,
    host: state.host
  }, function(err, stream) {
    if (err)
      return self.emit('error', err);

    stream.on('response', function(status, headers) {
      handle.emitResponse(status, headers);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.prototype._getCreateSocket"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_getCreateSocket ()](#apidoc.element.spdy.Agent.prototype._getCreateSocket)
- description and source-code
```javascript
function _getCreateSocket() {
  // Find super's 'createSocket' method
  var createSocket;
  var cons = this.constructor.super_;
  do {
    createSocket = cons.prototype.createSocket;

    if (cons.super_ === EventEmitter || !cons.super_)
      break;
    cons = cons.super_;
  } while (!createSocket);
  if (!createSocket)
    createSocket = http.Agent.prototype.createSocket;

  assert(createSocket, '.createSocket() method not found');

  return createSocket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.prototype._init"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>_init (base, options)](#apidoc.element.spdy.Agent.prototype._init)
- description and source-code
```javascript
function _init(base, options) {
  base.call(this, options);

  var state = {};
  this._spdyState = state;

  state.host = options.host;
  state.options = options.spdy || {};
  state.secure = this instanceof https.Agent;
  state.fallback = false;
  state.createSocket = this._getCreateSocket();
  state.socket = null;
  state.connection = null;

  // No chunked encoding
  this.keepAlive = false;

  var self = this;
  this._connect(options, function(err, connection) {
    if (err)
      return self.emit('error', err);

    state.connection = connection;
    self.emit('_connect');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.prototype.close"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>close (callback)](#apidoc.element.spdy.Agent.prototype.close)
- description and source-code
```javascript
function close(callback) {
  var state = this._spdyState;

  if (state.connection === null) {
    this.once('_connect', function() {
      this.close(callback);
    });
    return;
  }

  state.connection.end(callback);
}
```
- example usage
```shell
...
  agent: agent
}, function(response) {
  console.log('yikes');
  // Here it goes like with any other node.js HTTP request
  // ...
  // And once we're done - we may close TCP connection to server
  // NOTE: All non-closed requests will die!
  agent.close();
}).end();
'''

Please note that if you use a custom agent, by default all connection-level
errors will result in an uncaught exception. To handle these errors subscribe
to the 'error' event and re-emit the captured error:
...
```

#### <a name="apidoc.element.spdy.Agent.prototype.createSocket"></a>[function <span class="apidocSignatureSpan">spdy.Agent.prototype.</span>createSocket (req, options, callback)](#apidoc.element.spdy.Agent.prototype.createSocket)
- description and source-code
```javascript
function _createSocket(req, options, callback) {
  var state = this._spdyState;
  if (state.fallback)
    return state.createSocket(req, options);

  var handle = spdy.handle.create(null, null, state.socket);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(state.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);
  handle.assignClientRequest(req);

  // Create stream only once 'req.end()' is called
  var self = this;
  handle.once('needStream', function() {
    if (state.connection === null) {
      self.once('_connect', function() {
        handle.setStream(self._createStream(req, handle));
      });
    } else {
      handle.setStream(self._createStream(req, handle));
    }
  });

  // Yes, it is in reverse
  req.on('response', function(res) {
    handle.assignRequest(res);
  });
  handle.assignResponse(req);

  // Handle PUSH
  req.addListener('newListener', spdy.request.onNewListener);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  if (callback)
    return callback(null, socket);

  return socket;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Agent.super_"></a>[module spdy.Agent.super_](#apidoc.module.spdy.Agent.super_)

#### <a name="apidoc.element.spdy.Agent.super_.super_"></a>[function <span class="apidocSignatureSpan">spdy.Agent.</span>super_ (options)](#apidoc.element.spdy.Agent.super_.super_)
- description and source-code
```javascript
function Agent(options) {
  if (!(this instanceof Agent))
    return new Agent(options);

  EventEmitter.call(this);

  var self = this;

  self.defaultPort = 80;
  self.protocol = 'http:';

  self.options = util._extend({}, options);

  // don't confuse net and make it think that we're connecting to a pipe
  self.options.path = null;
  self.requests = {};
  self.sockets = {};
  self.freeSockets = {};
  self.keepAliveMsecs = self.options.keepAliveMsecs || 1000;
  self.keepAlive = self.options.keepAlive || false;
  self.maxSockets = self.options.maxSockets || Agent.defaultMaxSockets;
  self.maxFreeSockets = self.options.maxFreeSockets || 256;

  self.on('free', function(socket, options) {
    var name = self.getName(options);
    debug('agent.on(free)', name);

    if (socket.writable &&
        self.requests[name] && self.requests[name].length) {
      self.requests[name].shift().onSocket(socket);
      if (self.requests[name].length === 0) {
        // don't leak
        delete self.requests[name];
      }
    } else {
      // If there are no pending requests, then put it in
      // the freeSockets pool, but only if we're allowed to do so.
      var req = socket._httpMessage;
      if (req &&
          req.shouldKeepAlive &&
          socket.writable &&
          self.keepAlive) {
        var freeSockets = self.freeSockets[name];
        var freeLen = freeSockets ? freeSockets.length : 0;
        var count = freeLen;
        if (self.sockets[name])
          count += self.sockets[name].length;

        if (count > self.maxSockets || freeLen >= self.maxFreeSockets) {
          socket.destroy();
        } else {
          freeSockets = freeSockets || [];
          self.freeSockets[name] = freeSockets;
          socket.setKeepAlive(true, self.keepAliveMsecs);
          socket.unref();
          socket._httpMessage = null;
          self.removeSocket(socket, options);
          freeSockets.push(socket);
        }
      } else {
        socket.destroy();
      }
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Agent.super_.prototype"></a>[module spdy.Agent.super_.prototype](#apidoc.module.spdy.Agent.super_.prototype)

#### <a name="apidoc.element.spdy.Agent.super_.prototype._cacheSession"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_cacheSession (key, session)](#apidoc.element.spdy.Agent.super_.prototype._cacheSession)
- description and source-code
```javascript
function _cacheSession(key, session) {
  // Cache is disabled
  if (this.maxCachedSessions === 0)
    return;

  // Fast case - update existing entry
  if (this._sessionCache.map[key]) {
    this._sessionCache.map[key] = session;
    return;
  }

  // Put new entry
  if (this._sessionCache.list.length >= this.maxCachedSessions) {
    const oldKey = this._sessionCache.list.shift();
    debug('evicting %j', oldKey);
    delete this._sessionCache.map[oldKey];
  }

  this._sessionCache.list.push(key);
  this._sessionCache.map[key] = session;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.prototype._evictSession"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_evictSession (key)](#apidoc.element.spdy.Agent.super_.prototype._evictSession)
- description and source-code
```javascript
function _evictSession(key) {
  const index = this._sessionCache.list.indexOf(key);
  if (index === -1)
    return;

  this._sessionCache.list.splice(index, 1);
  delete this._sessionCache.map[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.prototype._getSession"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>_getSession (key)](#apidoc.element.spdy.Agent.super_.prototype._getSession)
- description and source-code
```javascript
function _getSession(key) {
  return this._sessionCache.map[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.prototype.createConnection"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>createConnection (port, host, options)](#apidoc.element.spdy.Agent.super_.prototype.createConnection)
- description and source-code
```javascript
function createConnection(port, host, options) {
  if (port !== null && typeof port === 'object') {
    options = port;
  } else if (host !== null && typeof host === 'object') {
    options = host;
  } else if (options === null || typeof options !== 'object') {
    options = {};
  }

  if (typeof port === 'number') {
    options.port = port;
  }

  if (typeof host === 'string') {
    options.host = host;
  }

  debug('createConnection', options);

  if (options._agentKey) {
    const session = this._getSession(options._agentKey);
    if (session) {
      debug('reuse session for %j', options._agentKey);
      options = util._extend({
        session: session
      }, options);
    }
  }

  const socket = tls.connect(options, () => {
    if (!options._agentKey)
      return;

    this._cacheSession(options._agentKey, socket.getSession());
  });

  // Evict session on error
  socket.once('close', (err) => {
    if (err)
      this._evictSession(options._agentKey);
  });

  return socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.prototype.getName"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.prototype.</span>getName (options)](#apidoc.element.spdy.Agent.super_.prototype.getName)
- description and source-code
```javascript
getName = function (options) {
  var name = http.Agent.prototype.getName.call(this, options);

  name += ':';
  if (options.ca)
    name += options.ca;

  name += ':';
  if (options.cert)
    name += options.cert;

  name += ':';
  if (options.ciphers)
    name += options.ciphers;

  name += ':';
  if (options.key)
    name += options.key;

  name += ':';
  if (options.pfx)
    name += options.pfx;

  name += ':';
  if (options.rejectUnauthorized !== undefined)
    name += options.rejectUnauthorized;

  name += ':';
  if (options.servername && options.servername !== options.host)
    name += options.servername;

  return name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Agent.super_.super_.prototype"></a>[module spdy.Agent.super_.super_.prototype](#apidoc.module.spdy.Agent.super_.super_.prototype)

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.addRequest"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>addRequest (req, options)](#apidoc.element.spdy.Agent.super_.super_.prototype.addRequest)
- description and source-code
```javascript
addRequest = function (req, options) {
  // Legacy API: addRequest(req, host, port, localAddress)
  if (typeof options === 'string') {
    options = {
      host: options,
      port: arguments[2],
      localAddress: arguments[3]
    };
  }

  options = util._extend({}, options);
  options = util._extend(options, this.options);

  if (!options.servername) {
    options.servername = options.host;
    const hostHeader = req.getHeader('host');
    if (hostHeader) {
      options.servername = hostHeader.replace(/:.*$/, '');
    }
  }

  var name = this.getName(options);
  if (!this.sockets[name]) {
    this.sockets[name] = [];
  }

  var freeLen = this.freeSockets[name] ? this.freeSockets[name].length : 0;
  var sockLen = freeLen + this.sockets[name].length;

  if (freeLen) {
    // we have a free socket, so use that.
    var socket = this.freeSockets[name].shift();
    debug('have free socket');

    // don't leak
    if (!this.freeSockets[name].length)
      delete this.freeSockets[name];

    socket.ref();
    req.onSocket(socket);
    this.sockets[name].push(socket);
  } else if (sockLen < this.maxSockets) {
    debug('call onSocket', sockLen, freeLen);
    // If we are under maxSockets create a new one.
    this.createSocket(req, options, function(err, newSocket) {
      if (err) {
        process.nextTick(function() {
          req.emit('error', err);
        });
        return;
      }
      req.onSocket(newSocket);
    });
  } else {
    debug('wait for socket');
    // We are over limit so we'll add it to the queue.
    if (!this.requests[name]) {
      this.requests[name] = [];
    }
    this.requests[name].push(req);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.createConnection"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>createConnection ()](#apidoc.element.spdy.Agent.super_.super_.prototype.createConnection)
- description and source-code
```javascript
createConnection = function () {
  var args = new Array(arguments.length);
  for (var i = 0; i < arguments.length; i++)
    args[i] = arguments[i];
  args = normalizeConnectArgs(args);
  debug('createConnection', args);
  var s = new Socket(args[0]);

  if (args[0].timeout) {
    s.setTimeout(args[0].timeout);
  }

  return Socket.prototype.connect.apply(s, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.createSocket"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>createSocket (req, options, cb)](#apidoc.element.spdy.Agent.super_.super_.prototype.createSocket)
- description and source-code
```javascript
createSocket = function (req, options, cb) {
  var self = this;
  options = util._extend({}, options);
  options = util._extend(options, self.options);

  if (!options.servername) {
    options.servername = options.host;
    const hostHeader = req.getHeader('host');
    if (hostHeader) {
      options.servername = hostHeader.replace(/:.*$/, '');
    }
  }

  var name = self.getName(options);
  options._agentKey = name;

  debug('createConnection', name, options);
  options.encoding = null;
  var called = false;
  const newSocket = self.createConnection(options, oncreate);
  if (newSocket)
    oncreate(null, newSocket);
  function oncreate(err, s) {
    if (called)
      return;
    called = true;
    if (err)
      return cb(err);
    if (!self.sockets[name]) {
      self.sockets[name] = [];
    }
    self.sockets[name].push(s);
    debug('sockets', name, self.sockets[name].length);

    function onFree() {
      self.emit('free', s, options);
    }
    s.on('free', onFree);

    function onClose(err) {
      debug('CLIENT socket onClose');
      // This is the only place where sockets get removed from the Agent.
      // If you want to remove a socket from the pool, just close it.
      // All socket errors end in a close event anyway.
      self.removeSocket(s, options);
    }
    s.on('close', onClose);

    function onRemove() {
      // We need this function for cases like HTTP 'upgrade'
      // (defined by WebSockets) where we need to remove a socket from the
      // pool because it'll be locked up indefinitely
      debug('CLIENT socket onRemove');
      self.removeSocket(s, options);
      s.removeListener('close', onClose);
      s.removeListener('free', onFree);
      s.removeListener('agentRemove', onRemove);
    }
    s.on('agentRemove', onRemove);
    cb(null, s);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.destroy"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>destroy ()](#apidoc.element.spdy.Agent.super_.super_.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var sets = [this.freeSockets, this.sockets];
  for (var s = 0; s < sets.length; s++) {
    var set = sets[s];
    var keys = Object.keys(set);
    for (var v = 0; v < keys.length; v++) {
      var setName = set[keys[v]];
      for (var n = 0; n < setName.length; n++) {
        setName[n].destroy();
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.getName"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>getName (options)](#apidoc.element.spdy.Agent.super_.super_.prototype.getName)
- description and source-code
```javascript
getName = function (options) {
  var name = options.host || 'localhost';

  name += ':';
  if (options.port)
    name += options.port;

  name += ':';
  if (options.localAddress)
    name += options.localAddress;

  // Pacify parallel/test-http-agent-getname by only appending
  // the ':' when options.family is set.
  if (options.family === 4 || options.family === 6)
    name += ':' + options.family;

  return name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Agent.super_.super_.prototype.removeSocket"></a>[function <span class="apidocSignatureSpan">spdy.Agent.super_.super_.prototype.</span>removeSocket (s, options)](#apidoc.element.spdy.Agent.super_.super_.prototype.removeSocket)
- description and source-code
```javascript
removeSocket = function (s, options) {
  var name = this.getName(options);
  debug('removeSocket', name, 'writable:', s.writable);
  var sets = [this.sockets];

  // If the socket was destroyed, remove it from the free buffers too.
  if (!s.writable)
    sets.push(this.freeSockets);

  for (var sk = 0; sk < sets.length; sk++) {
    var sockets = sets[sk];

    if (sockets[name]) {
      var index = sockets[name].indexOf(s);
      if (index !== -1) {
        sockets[name].splice(index, 1);
        // Don't leak
        if (sockets[name].length === 0)
          delete sockets[name];
      }
    }
  }

  if (this.requests[name] && this.requests[name].length) {
    debug('removeSocket, have a request, make a socket');
    var req = this.requests[name][0];
    // If we have pending requests and a socket gets closed make a new one
    this.createSocket(req, options, function(err, newSocket) {
      if (err) {
        process.nextTick(function() {
          req.emit('error', err);
        });
        return;
      }
      newSocket.emit('free');
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.PlainServer"></a>[module spdy.PlainServer](#apidoc.module.spdy.PlainServer)

#### <a name="apidoc.element.spdy.PlainServer.PlainServer"></a>[function <span class="apidocSignatureSpan">spdy.</span>PlainServer (options, handler)](#apidoc.element.spdy.PlainServer.PlainServer)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.create"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.</span>create (options, handler)](#apidoc.element.spdy.PlainServer.create)
- description and source-code
```javascript
function create(options, handler) {
  return new Server(options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.</span>super_ (requestListener)](#apidoc.element.spdy.PlainServer.super_)
- description and source-code
```javascript
function Server(requestListener) {
  if (!(this instanceof Server)) return new Server(requestListener);
  net.Server.call(this, { allowHalfOpen: true });

  if (requestListener) {
    this.addListener('request', requestListener);
  }

<span class="apidocCodeCommentSpan">  /* eslint-disable max-len */
</span>  // Similar option to this. Too lazy to write my own docs.
  // http://www.squid-cache.org/Doc/config/half_closed_clients/
  // http://wiki.squid-cache.org/SquidFaq/InnerWorkings#What_is_a_half-closed_filedescriptor.3F
  /* eslint-enable max-len */
  this.httpAllowHalfOpen = false;

  this.addListener('connection', connectionListener);

  this.timeout = 2 * 60 * 1000;

  this._pendingResponseData = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.PlainServer.prototype"></a>[module spdy.PlainServer.prototype](#apidoc.module.spdy.PlainServer.prototype)

#### <a name="apidoc.element.spdy.PlainServer.prototype._handleConnection"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_handleConnection (socket, protocol)](#apidoc.element.spdy.PlainServer.prototype._handleConnection)
- description and source-code
```javascript
function _handleConnection(socket, protocol) {
  var state = this._spdyState;

  if (!protocol)
    protocol = state.options.protocol;

  debug('incoming socket protocol=%j', protocol);

  // No way we can do anything with the socket
  if (!protocol || protocol === 'http/1.1' || protocol === 'http/1.0') {
    debug('to default handler it goes');
    return this._invokeDefault(socket);
  }

  socket.setNoDelay(true);

  var connection = transport.connection.create(socket, util._extend({
    protocol: /spdy/.test(protocol) ? 'spdy' : 'http2',
    isServer: true
  }, state.options.connection || {}));

  // Set version when we are certain
  if (protocol === 'http2')
    connection.start(4);
  else if (protocol === 'spdy/3.1')
    connection.start(3.1);
  else if (protocol === 'spdy/3')
    connection.start(3);
  else if (protocol === 'spdy/2')
    connection.start(2);

  connection.on('error', function() {
    socket.destroy();
  });

  var self = this;
  connection.on('stream', function(stream) {
    self._onStream(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype._init"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_init (base, options, handler)](#apidoc.element.spdy.PlainServer.prototype._init)
- description and source-code
```javascript
function _init(base, options, handler) {
  var state = {};
  this._spdyState = state;

  state.options = options.spdy || {};

  var protocols = state.options.protocols || [
    'h2',
    'spdy/3.1', 'spdy/3', 'spdy/2',
    'http/1.1', 'http/1.0'
  ];

  var actualOptions = util._extend({
    NPNProtocols: protocols,

    // Future-proof
    ALPNProtocols: protocols
  }, options);

  state.secure = this instanceof tls.Server;

  if (state.secure)
    base.call(this, actualOptions);
  else
    base.call(this);

  // Support HEADERS+FIN
  this.httpAllowHalfOpen = true;

  var event = state.secure ? 'secureConnection' : 'connection';

  state.listeners = this.listeners(event).slice();
  assert(state.listeners.length > 0, 'Server does not have default listeners');
  this.removeAllListeners(event);

  if (state.options.plain)
    this.on(event, this._onPlainConnection);
  else
    this.on(event, this._onConnection);

  if (handler)
    this.on('request', handler);

  debug('server init secure=%d', state.secure);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype._invokeDefault"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_invokeDefault (socket)](#apidoc.element.spdy.PlainServer.prototype._invokeDefault)
- description and source-code
```javascript
function _invokeDefault(socket) {
  var state = this._spdyState;

  for (var i = 0; i < state.listeners.length; i++)
    state.listeners[i].call(this, socket);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype._onConnection"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onConnection (socket)](#apidoc.element.spdy.PlainServer.prototype._onConnection)
- description and source-code
```javascript
function _onConnection(socket) {
  var state = this._spdyState;

  var protocol;
  if (state.secure)
    protocol = socket.npnProtocol || socket.alpnProtocol;

  this._handleConnection(socket, protocol);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype._onPlainConnection"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onPlainConnection (socket)](#apidoc.element.spdy.PlainServer.prototype._onPlainConnection)
- description and source-code
```javascript
function _onPlainConnection(socket) {
  var hose = selectHose.create(socket, {}, hoseFilter);

  var self = this;
  hose.on('select', function(protocol, socket) {
    self._handleConnection(socket, protocol);
  });

  hose.on('error', function(err) {
    debug('hose error %j', err.message);
    socket.destroy();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype._onStream"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>_onStream (stream)](#apidoc.element.spdy.PlainServer.prototype._onStream)
- description and source-code
```javascript
function _onStream(stream) {
  var state = this._spdyState;

  var handle = spdy.handle.create(this._spdyState.options, stream);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(stream.connection.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  this._invokeDefault(socket);

  // Add lazy 'checkContinue' listener, otherwise 'res.writeContinue' will be
  // called before the response object was patched by us.
  if (stream.headers.expect !== undefined &&
      /100-continue/i.test(stream.headers.expect) &&
      EventEmitter.listenerCount(this, 'checkContinue') === 0) {
    this.once('checkContinue', function(req, res) {
      res.writeContinue();

      this.emit('request', req, res);
    });
  }

  handle.emitRequest();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.prototype.emit"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.prototype.</span>emit (event, req, res)](#apidoc.element.spdy.PlainServer.prototype.emit)
- description and source-code
```javascript
function emit(event, req, res) {
  if (event !== 'request' && event !== 'checkContinue')
    return EventEmitter.prototype.emit.apply(this, arguments);

  if (!(req.socket._handle instanceof spdy.handle)) {
    debug('not spdy req/res');
    req.isSpdy = false;
    req.spdyVersion = 1;
    res.isSpdy = false;
    res.spdyVersion = 1;
    return EventEmitter.prototype.emit.apply(this, arguments);
  }

  var handle = req.connection._handle;

  req.isSpdy = true;
  req.spdyVersion = handle.getStream().connection.getVersion();
  res.isSpdy = true;
  res.spdyVersion = req.spdyVersion;
  req.spdyStream = handle.getStream();

  debug('override req/res');
  res.writeHead = spdy.response.writeHead;
  res.end = spdy.response.end;
  res.push = spdy.response.push;
  res.writeContinue = spdy.response.writeContinue;
  res.spdyStream = handle.getStream();

  res._req = req;

  handle.assignRequest(req);
  handle.assignResponse(res);

  return EventEmitter.prototype.emit.apply(this, arguments);
}
```
- example usage
```shell
...
to the 'error' event and re-emit the captured error:

'''javascript
var agent = spdy.createAgent({
  host: 'www.google.com',
  port: 443
}).once('error', function (err) {
  this.emit(err);
});
'''

## API

API is compatible with 'http' and 'https' module, but you can use another
function as base class for SPDYServer.
...
```



# <a name="apidoc.module.spdy.PlainServer.super_"></a>[module spdy.PlainServer.super_](#apidoc.module.spdy.PlainServer.super_)

#### <a name="apidoc.element.spdy.PlainServer.super_.super_"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.</span>super_ (options, connectionListener)](#apidoc.element.spdy.PlainServer.super_.super_)
- description and source-code
```javascript
function Server(options, connectionListener) {
  if (!(this instanceof Server))
    return new Server(options, connectionListener);

  EventEmitter.call(this);

  if (typeof options === 'function') {
    connectionListener = options;
    options = {};
    this.on('connection', connectionListener);
  } else if (options == null || typeof options === 'object') {
    options = options || {};

    if (typeof connectionListener === 'function') {
      this.on('connection', connectionListener);
    }
  } else {
    throw new TypeError('options must be an object');
  }

  this._connections = 0;

  Object.defineProperty(this, 'connections', {
    get: internalUtil.deprecate(() => {

      if (this._usingSlaves) {
        return null;
      }
      return this._connections;
    }, 'Server.connections property is deprecated. ' +
       'Use Server.getConnections method instead.'),
    set: internalUtil.deprecate((val) => {
      return (this._connections = val);
    }, 'Server.connections property is deprecated.'),
    configurable: true, enumerable: false
  });

  this._handle = null;
  this._usingSlaves = false;
  this._slaves = [];
  this._unref = false;

  this.allowHalfOpen = options.allowHalfOpen || false;
  this.pauseOnConnect = !!options.pauseOnConnect;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.PlainServer.super_.prototype"></a>[module spdy.PlainServer.super_.prototype](#apidoc.module.spdy.PlainServer.super_.prototype)

#### <a name="apidoc.element.spdy.PlainServer.super_.prototype.setTimeout"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.PlainServer.super_.prototype.setTimeout)
- description and source-code
```javascript
setTimeout = function (msecs, callback) {
  this.timeout = msecs;
  if (callback)
    this.on('timeout', callback);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.PlainServer.super_.super_.prototype"></a>[module spdy.PlainServer.super_.super_.prototype](#apidoc.module.spdy.PlainServer.super_.super_.prototype)

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype._emitCloseIfDrained"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_emitCloseIfDrained ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype._emitCloseIfDrained)
- description and source-code
```javascript
_emitCloseIfDrained = function () {
  debug('SERVER _emitCloseIfDrained');

  if (this._handle || this._connections) {
    debug('SERVER handle? %j   connections? %d',
          !!this._handle, this._connections);
    return;
  }

  process.nextTick(emitCloseNT, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype._listen2"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_listen2 (address, port, addressType, backlog, fd)](#apidoc.element.spdy.PlainServer.super_.super_.prototype._listen2)
- description and source-code
```javascript
_listen2 = function (address, port, addressType, backlog, fd) {
  debug('listen2', address, port, addressType, backlog, fd);

  // If there is not yet a handle, we need to create one and bind.
  // In the case of a server sent via IPC, we don't need to do this.
  if (this._handle) {
    debug('_listen2: have a handle already');
  } else {
    debug('_listen2: create a handle');

    var rval = null;

    if (!address && typeof fd !== 'number') {
      rval = createServerHandle('::', port, 6, fd);

      if (typeof rval === 'number') {
        rval = null;
        address = '0.0.0.0';
        addressType = 4;
      } else {
        address = '::';
        addressType = 6;
      }
    }

    if (rval === null)
      rval = createServerHandle(address, port, addressType, fd);

    if (typeof rval === 'number') {
      var error = exceptionWithHostPort(rval, 'listen', address, port);
      process.nextTick(emitErrorNT, this, error);
      return;
    }
    this._handle = rval;
  }

  this._handle.onconnection = onconnection;
  this._handle.owner = this;

  var err = _listen(this._handle, backlog);

  if (err) {
    var ex = exceptionWithHostPort(err, 'listen', address, port);
    this._handle.close();
    this._handle = null;
    process.nextTick(emitErrorNT, this, ex);
    return;
  }

  // generate connection key, this should be unique to the connection
  this._connectionKey = addressType + ':' + address + ':' + port;

  // unref the handle if the server was unref'ed prior to listening
  if (this._unref)
    this.unref();

  process.nextTick(emitListeningNT, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype._setupSlave"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>_setupSlave (socketList)](#apidoc.element.spdy.PlainServer.super_.super_.prototype._setupSlave)
- description and source-code
```javascript
_setupSlave = function (socketList) {
  this._usingSlaves = true;
  this._slaves.push(socketList);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.address"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>address ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.address)
- description and source-code
```javascript
address = function () {
  if (this._handle && this._handle.getsockname) {
    var out = {};
    this._handle.getsockname(out);
    // TODO(bnoordhuis) Check err and throw?
    return out;
  } else if (this._pipeName) {
    return this._pipeName;
  } else {
    return null;
  }
}
```
- example usage
```shell
...
  key: "-----BEGIN RSA PRIVATE KEY-----\nMIIEpAIBAAKCAQEA4YyUIzAnCuSz43HXIPfX60XTeXJLYZZXHnyJIXdBkgE2Ou0F\nhWg0wgbicSiyCoRVQHdFcWhIYQRCq2qu3YKetRxD
/MNY9X0h0cPwf3vYP0Bqowhz\neXPc9DoUl0IwbbolYeHlchgm59w9y/UrjO8fEXxhiBpZnllR2N8C0J6p0T9Itn9y\nxN0iWOuZonrvC8upBquniDnW8X5jwTMUEMbCKBQsVoHZm7R+wfX6BfWTUDGFDh1s\norgMqFarP8TRMYqCFUfM/DFS1CeicpvN6i9SixmboIudSRXOHA+FCh0MrW+JxjDt\nBGHq3AZP0y5+f5ETQvtCWBR1xhv3fHGILshiMQIDAQABAoIBAETE5g3siprprGd2\nuE8XAkB748StsooomptzASSxBc8Mi4pf5kUMxrk5/CTgcZh/TLcBJq0zTI44DFPT\njUmAn/88hQY2UZNX+c3JXjSggAiZDWp0EzE+wGm+o7SSu81Y6jjz9U9aSdJ79mOP\ndx3bcq+UKvCiiBydwzTKmkMdfU2M2Wh/LVerXIlO5P4GsEsbenf53iafj0sHOY4W\n8mf1cWHl8/N+5Eh+0GDIIITGOjmGqNKLZOOg66wjzdY9WbCMTJUWIUjRHjCoG6ZA\nJz+vdsZQVN7M4zy8/fKkE4Vx9NEoJcDfZYa/4uo9r274TK7pJD448nTgRCKOJfMR\nCuxZHXkCgYEA5obXLtRiYXhHyXZOs/Yu9/1Iwm6zHiU66/eFRNGHzTssbPSle1kK\n/2LI3+xiRTI8PfztVP6br5/cWLKhu1ZVebCn+wJJbhpHTfAw1k1YXaCjwHh2l1OF\nPBbT4BPjK2ELNzMMF8veLY6S4yY3bQn8xUmbjQtOYuKDvFgoYAsXQo8CgYEA+nju\nhqAXSDW9yoYQBAXoduEaQH2qNfwRzY6V8rkwISI1seLPlcsd0Kc/VDOSwRdCWOk2\njn5LKPql6FfZ+9MVtPjlVLFjLcEzXttH+PkFtoA9Ffj9cxe3owNjR/tbfoHa19pV\n6+vBZJF48AlkErmVzTNlFJGWh7GtY6LgaOwdbz8CgYEAwhFaLe5WNEASDyQt9YqW\n1+a+zhBrckFdbTEfXGQYs0nRiJgch87aV01OVlSmFiLIXFcFZbxCTIOD+JfJV/DC\nXIO/pqyyLKKqzI4cTw0mCwwlTu8axyJk08VT8RxM7kPwMTQkRhQ2opuYROnzVzRF\nO8FP1lliUBTpWjHNK62qkzkCgYBZg+rLVl+7wOkpfiwvI+VmxyBYuBCi5ol+S10v\nuBuJW+6QupyxzjvDnGI3t47VT3i4yfBjkKNP6/RrSypuo4v4d5OOZy8o5Ql09y2L\nv4PZK4+pUKlT/r/0lHtg+GZEmigaSL+4ZzNgu9TbBKAtSQJOqfWQGlAQAuIS390P\n4oLKhQKBgQDiuimWRSpW3vBepzeH3SuJqm5yx/ms5RUdFH1tc/0vMZR9x/c4Ai2r\ns+1E3KacY/5z9D6t5PWaDj5Sbw8dz0zI7nvnIvufznaaGGqWlrPACQndQLnPrPSr\niFltJhhNQAMlAVOeOz75IQGuC4swdXxbdWXXPrmN9VKGPjClqU+/+w==\n-----END RSA PRIVATE KEY-----",
  cert: "-----BEGIN CERTIFICATE-----\nMIICvDCCAaagAwIBAgIDAQABMAsGCSqGSIb3DQEBDTAVMRMwEQYDVQQDFgpsb2Nh\nbC5ob3N0MB4XDTE2MDkxNzE5MDEyOVoXDTI2MDkxNjE5MDEyOVowFTETMBEGA1UE\nAxYKbG9jYWwuaG9zdDCCASAwCwYJKoZIhvcNAQEBA4IBDwAwggEKAoIBAQDhjJQj\nMCcK5LPjcdcg99frRdN5ckthllcefIkhd0GSATY67QWFaDTCBuJxKLIKhFVAd0Vx\naEhhBEKraq7dgp61HEP8w1j1fSHRw/B/e9g/QGqjCHN5c9z0OhSXQjBtuiVh4eVy\nGCbn3D3L9SuM7x8RfGGIGlmeWVHY3wLQnqnRP0i2f3LE3SJY65mieu8Ly6kGq6eI\nOdbxfmPBMxQQxsIoFCxWgdmbtH7B9foF9ZNQMYUOHWyiuAyoVqs/xNExioIVR8z8\nMVLUJ6Jym83qL1KLGZugi51JFc4cD4UKHQytb4nGMO0EYercBk/TLn5/kRNC+0JY\nFHXGG/d8cYguyGIxAgMBAAGjGzAZMBcGA1UdEQQQMA6CDCoubG9jYWwuaG9zdDAL\nBgkqhkiG9w0BAQ0DggEBAHX840Wl7APZi20i+H+eSL70/tGfld487CBnxfzvECWh\nC+mOfMH9LHSkRhkk+kyosClKO07moUev39EppR7rXhh/fDJLUAbH8Hpb8gJBu0R6\nceQQmqoHCFApqdDF0quvKq5RVatQHfTTuSNd2y/kPD6otnEfxk91rg10dpwd0jii\nv7JBV8cC+z6bDBKn46P8Hpy0k2AY8LgIpUdnmLecxcPAGh0TpGe/2FuYtvPey7vR\nKl4sqjtreZ5kbrqoKRGTU/X2bXHjhF22ZmWO/O0lv1rLrnXCnxQrSTwvXHfNsxkZ\nVqvOQufB7zDfcVrXAeQr7RpyP9qSF9aQwDQj8uio/dI=\n-----END CERTIFICATE-----"
};

const server = spdy.createServer(options, (req, res) => {
  res.end('hello');
}).listen(443, () => {
  console.log('Listening', server.address());
});
...
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>close (cb)](#apidoc.element.spdy.PlainServer.super_.super_.prototype.close)
- description and source-code
```javascript
close = function (cb) {
  function onSlaveClose() {
    if (--left !== 0) return;

    self._connections = 0;
    self._emitCloseIfDrained();
  }

  if (typeof cb === 'function') {
    if (!this._handle) {
      this.once('close', function() {
        cb(new Error('Not running'));
      });
    } else {
      this.once('close', cb);
    }
  }

  if (this._handle) {
    this._handle.close();
    this._handle = null;
  }

  if (this._usingSlaves) {
    var self = this;
    var left = this._slaves.length;

    // Increment connections to be sure that, even if all sockets will be closed
    // during polling of slaves, 'close' event will be emitted only once.
    this._connections++;

    // Poll slaves
    this._slaves.forEach(function(slave) {
      slave.close(onSlaveClose);
    });
  } else {
    this._emitCloseIfDrained();
  }

  return this;
}
```
- example usage
```shell
...
  agent: agent
}, function(response) {
  console.log('yikes');
  // Here it goes like with any other node.js HTTP request
  // ...
  // And once we're done - we may close TCP connection to server
  // NOTE: All non-closed requests will die!
  agent.close();
}).end();
'''

Please note that if you use a custom agent, by default all connection-level
errors will result in an uncaught exception. To handle these errors subscribe
to the 'error' event and re-emit the captured error:
...
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.getConnections"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>getConnections (cb)](#apidoc.element.spdy.PlainServer.super_.super_.prototype.getConnections)
- description and source-code
```javascript
getConnections = function (cb) {
  function end(err, connections) {
    process.nextTick(cb, err, connections);
  }

  if (!this._usingSlaves) {
    return end(null, this._connections);
  }

  // Poll slaves
  var left = this._slaves.length;
  var total = this._connections;

  function oncount(err, count) {
    if (err) {
      left = -1;
      return end(err);
    }

    total += count;
    if (--left === 0) return end(null, total);
  }

  this._slaves.forEach(function(slave) {
    slave.getConnections(oncount);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.listen"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>listen ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.listen)
- description and source-code
```javascript
listen = function () {
  var self = this;

  var lastArg = arguments[arguments.length - 1];
  if (typeof lastArg === 'function') {
    self.once('listening', lastArg);
  }

  var port = toNumber(arguments[0]);

  // The third optional argument is the backlog size.
  // When the ip is omitted it can be the second argument.
  var backlog = toNumber(arguments[1]) || toNumber(arguments[2]);

  if (arguments.length === 0 || typeof arguments[0] === 'function') {
    // Bind to a random port.
    listen(self, null, 0, null, backlog);
  } else if (arguments[0] !== null && typeof arguments[0] === 'object') {
    var h = arguments[0];
    h = h._handle || h.handle || h;

    if (h instanceof TCP) {
      self._handle = h;
      listen(self, null, -1, -1, backlog);
    } else if (typeof h.fd === 'number' && h.fd >= 0) {
      listen(self, null, null, null, backlog, h.fd);
    } else {
      // The first argument is a configuration object
      if (h.backlog)
        backlog = h.backlog;

      if (typeof h.port === 'number' || typeof h.port === 'string' ||
          (typeof h.port === 'undefined' && 'port' in h)) {
        // Undefined is interpreted as zero (random port) for consistency
        // with net.connect().
        assertPort(h.port);
        if (h.host)
          listenAfterLookup(h.port | 0, h.host, backlog, h.exclusive);
        else
          listen(self, null, h.port | 0, 4, backlog, undefined, h.exclusive);
      } else if (h.path && isPipeName(h.path)) {
        const pipeName = self._pipeName = h.path;
        listen(self, pipeName, -1, -1, backlog, undefined, h.exclusive);
      } else {
        throw new Error('Invalid listen argument: ' + h);
      }
    }
  } else if (isPipeName(arguments[0])) {
    // UNIX socket or Windows pipe.
    const pipeName = self._pipeName = arguments[0];
    listen(self, pipeName, -1, -1, backlog);

  } else if (arguments[1] === undefined ||
             typeof arguments[1] === 'function' ||
             typeof arguments[1] === 'number') {
    // The first argument is the port, no IP given.
    assertPort(port);
    listen(self, null, port, 4, backlog);

  } else {
    // The first argument is the port, the second an IP.
    assertPort(port);
    listenAfterLookup(port, arguments[1], backlog);
  }

  function listenAfterLookup(port, address, backlog, exclusive) {
    require('dns').lookup(address, function(err, ip, addressType) {
      if (err) {
        self.emit('error', err);
      } else {
        addressType = ip ? addressType : 4;
        listen(self, ip, port, addressType, backlog, undefined, exclusive);
      }
    });
  }

  return self;
}
```
- example usage
```shell
...
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''

Client:
'''javascript
var spdy = require('spdy');
var http = require('http');
...
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.listenFD"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>listenFD ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.listenFD)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.ref"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>ref ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.ref)
- description and source-code
```javascript
ref = function () {
  this._unref = false;

  if (this._handle)
    this._handle.ref();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.PlainServer.super_.super_.prototype.unref"></a>[function <span class="apidocSignatureSpan">spdy.PlainServer.super_.super_.prototype.</span>unref ()](#apidoc.element.spdy.PlainServer.super_.super_.prototype.unref)
- description and source-code
```javascript
unref = function () {
  this._unref = true;

  if (this._handle)
    this._handle.unref();

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Server"></a>[module spdy.Server](#apidoc.module.spdy.Server)

#### <a name="apidoc.element.spdy.Server.Server"></a>[function <span class="apidocSignatureSpan">spdy.</span>Server (options, handler)](#apidoc.element.spdy.Server.Server)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.create"></a>[function <span class="apidocSignatureSpan">spdy.Server.</span>create (options, handler)](#apidoc.element.spdy.Server.create)
- description and source-code
```javascript
function create(options, handler) {
  return new Server(options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_"></a>[function <span class="apidocSignatureSpan">spdy.Server.</span>super_ (opts, requestListener)](#apidoc.element.spdy.Server.super_)
- description and source-code
```javascript
function Server(opts, requestListener) {
  if (!(this instanceof Server)) return new Server(opts, requestListener);

  if (process.features.tls_npn && !opts.NPNProtocols) {
    opts.NPNProtocols = ['http/1.1', 'http/1.0'];
  }

  if (process.features.tls_alpn && !opts.ALPNProtocols) {
    // http/1.0 is not defined as Protocol IDs in IANA
    // http://www.iana.org/assignments/tls-extensiontype-values
    //       /tls-extensiontype-values.xhtml#alpn-protocol-ids
    opts.ALPNProtocols = ['http/1.1'];
  }

  tls.Server.call(this, opts, http._connectionListener);

  this.httpAllowHalfOpen = false;

  if (requestListener) {
    this.addListener('request', requestListener);
  }

  this.addListener('tlsClientError', function(err, conn) {
    if (!this.emit('clientError', err, conn))
      conn.destroy(err);
  });

  this.timeout = 2 * 60 * 1000;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Server.prototype"></a>[module spdy.Server.prototype](#apidoc.module.spdy.Server.prototype)

#### <a name="apidoc.element.spdy.Server.prototype._handleConnection"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_handleConnection (socket, protocol)](#apidoc.element.spdy.Server.prototype._handleConnection)
- description and source-code
```javascript
function _handleConnection(socket, protocol) {
  var state = this._spdyState;

  if (!protocol)
    protocol = state.options.protocol;

  debug('incoming socket protocol=%j', protocol);

  // No way we can do anything with the socket
  if (!protocol || protocol === 'http/1.1' || protocol === 'http/1.0') {
    debug('to default handler it goes');
    return this._invokeDefault(socket);
  }

  socket.setNoDelay(true);

  var connection = transport.connection.create(socket, util._extend({
    protocol: /spdy/.test(protocol) ? 'spdy' : 'http2',
    isServer: true
  }, state.options.connection || {}));

  // Set version when we are certain
  if (protocol === 'http2')
    connection.start(4);
  else if (protocol === 'spdy/3.1')
    connection.start(3.1);
  else if (protocol === 'spdy/3')
    connection.start(3);
  else if (protocol === 'spdy/2')
    connection.start(2);

  connection.on('error', function() {
    socket.destroy();
  });

  var self = this;
  connection.on('stream', function(stream) {
    self._onStream(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype._init"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_init (base, options, handler)](#apidoc.element.spdy.Server.prototype._init)
- description and source-code
```javascript
function _init(base, options, handler) {
  var state = {};
  this._spdyState = state;

  state.options = options.spdy || {};

  var protocols = state.options.protocols || [
    'h2',
    'spdy/3.1', 'spdy/3', 'spdy/2',
    'http/1.1', 'http/1.0'
  ];

  var actualOptions = util._extend({
    NPNProtocols: protocols,

    // Future-proof
    ALPNProtocols: protocols
  }, options);

  state.secure = this instanceof tls.Server;

  if (state.secure)
    base.call(this, actualOptions);
  else
    base.call(this);

  // Support HEADERS+FIN
  this.httpAllowHalfOpen = true;

  var event = state.secure ? 'secureConnection' : 'connection';

  state.listeners = this.listeners(event).slice();
  assert(state.listeners.length > 0, 'Server does not have default listeners');
  this.removeAllListeners(event);

  if (state.options.plain)
    this.on(event, this._onPlainConnection);
  else
    this.on(event, this._onConnection);

  if (handler)
    this.on('request', handler);

  debug('server init secure=%d', state.secure);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype._invokeDefault"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_invokeDefault (socket)](#apidoc.element.spdy.Server.prototype._invokeDefault)
- description and source-code
```javascript
function _invokeDefault(socket) {
  var state = this._spdyState;

  for (var i = 0; i < state.listeners.length; i++)
    state.listeners[i].call(this, socket);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype._onConnection"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onConnection (socket)](#apidoc.element.spdy.Server.prototype._onConnection)
- description and source-code
```javascript
function _onConnection(socket) {
  var state = this._spdyState;

  var protocol;
  if (state.secure)
    protocol = socket.npnProtocol || socket.alpnProtocol;

  this._handleConnection(socket, protocol);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype._onPlainConnection"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onPlainConnection (socket)](#apidoc.element.spdy.Server.prototype._onPlainConnection)
- description and source-code
```javascript
function _onPlainConnection(socket) {
  var hose = selectHose.create(socket, {}, hoseFilter);

  var self = this;
  hose.on('select', function(protocol, socket) {
    self._handleConnection(socket, protocol);
  });

  hose.on('error', function(err) {
    debug('hose error %j', err.message);
    socket.destroy();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype._onStream"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>_onStream (stream)](#apidoc.element.spdy.Server.prototype._onStream)
- description and source-code
```javascript
function _onStream(stream) {
  var state = this._spdyState;

  var handle = spdy.handle.create(this._spdyState.options, stream);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(stream.connection.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  this._invokeDefault(socket);

  // Add lazy 'checkContinue' listener, otherwise 'res.writeContinue' will be
  // called before the response object was patched by us.
  if (stream.headers.expect !== undefined &&
      /100-continue/i.test(stream.headers.expect) &&
      EventEmitter.listenerCount(this, 'checkContinue') === 0) {
    this.once('checkContinue', function(req, res) {
      res.writeContinue();

      this.emit('request', req, res);
    });
  }

  handle.emitRequest();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.prototype.emit"></a>[function <span class="apidocSignatureSpan">spdy.Server.prototype.</span>emit (event, req, res)](#apidoc.element.spdy.Server.prototype.emit)
- description and source-code
```javascript
function emit(event, req, res) {
  if (event !== 'request' && event !== 'checkContinue')
    return EventEmitter.prototype.emit.apply(this, arguments);

  if (!(req.socket._handle instanceof spdy.handle)) {
    debug('not spdy req/res');
    req.isSpdy = false;
    req.spdyVersion = 1;
    res.isSpdy = false;
    res.spdyVersion = 1;
    return EventEmitter.prototype.emit.apply(this, arguments);
  }

  var handle = req.connection._handle;

  req.isSpdy = true;
  req.spdyVersion = handle.getStream().connection.getVersion();
  res.isSpdy = true;
  res.spdyVersion = req.spdyVersion;
  req.spdyStream = handle.getStream();

  debug('override req/res');
  res.writeHead = spdy.response.writeHead;
  res.end = spdy.response.end;
  res.push = spdy.response.push;
  res.writeContinue = spdy.response.writeContinue;
  res.spdyStream = handle.getStream();

  res._req = req;

  handle.assignRequest(req);
  handle.assignResponse(res);

  return EventEmitter.prototype.emit.apply(this, arguments);
}
```
- example usage
```shell
...
to the 'error' event and re-emit the captured error:

'''javascript
var agent = spdy.createAgent({
  host: 'www.google.com',
  port: 443
}).once('error', function (err) {
  this.emit(err);
});
'''

## API

API is compatible with 'http' and 'https' module, but you can use another
function as base class for SPDYServer.
...
```



# <a name="apidoc.module.spdy.Server.super_"></a>[module spdy.Server.super_](#apidoc.module.spdy.Server.super_)

#### <a name="apidoc.element.spdy.Server.super_.super_"></a>[function <span class="apidocSignatureSpan">spdy.Server.</span>super_ (options, listener)](#apidoc.element.spdy.Server.super_.super_)
- description and source-code
```javascript
function Server(options, listener) {
  if (!(this instanceof Server))
    return new Server(options, listener);

  if (typeof options === 'function') {
    listener = options;
    options = {};
  } else if (options == null || typeof options === 'object') {
    options = options || {};
  } else {
    throw new TypeError('options must be an object');
  }


  this._contexts = [];

  var self = this;

  // Handle option defaults:
  this.setOptions(options);

  var sharedCreds = tls.createSecureContext({
    pfx: self.pfx,
    key: self.key,
    passphrase: self.passphrase,
    cert: self.cert,
    ca: self.ca,
    ciphers: self.ciphers,
    ecdhCurve: self.ecdhCurve,
    dhparam: self.dhparam,
    secureProtocol: self.secureProtocol,
    secureOptions: self.secureOptions,
    honorCipherOrder: self.honorCipherOrder,
    crl: self.crl,
    sessionIdContext: self.sessionIdContext
  });
  this._sharedCreds = sharedCreds;

  var timeout = options.handshakeTimeout || (120 * 1000);

  if (typeof timeout !== 'number') {
    throw new TypeError('handshakeTimeout must be a number');
  }

  if (self.sessionTimeout) {
    sharedCreds.context.setSessionTimeout(self.sessionTimeout);
  }

  if (self.ticketKeys) {
    sharedCreds.context.setTicketKeys(self.ticketKeys);
  }

  // constructor call
  net.Server.call(this, function(raw_socket) {
    var socket = new TLSSocket(raw_socket, {
      secureContext: sharedCreds,
      isServer: true,
      server: self,
      requestCert: self.requestCert,
      rejectUnauthorized: self.rejectUnauthorized,
      handshakeTimeout: timeout,
      NPNProtocols: self.NPNProtocols,
      ALPNProtocols: self.ALPNProtocols,
      SNICallback: options.SNICallback || SNICallback
    });

    socket.on('secure', function() {
      if (socket._requestCert) {
        var verifyError = socket._handle.verifyError();
        if (verifyError) {
          socket.authorizationError = verifyError.code;

          if (socket._rejectUnauthorized)
            socket.destroy();
        } else {
          socket.authorized = true;
        }
      }

      if (!socket.destroyed && socket._releaseControl())
        self.emit('secureConnection', socket);
    });

    var errorEmitted = false;
    socket.on('close', function(err) {
      // Closed because of error - no need to emit it twice
      if (err)
        return;

      // Emit ECONNRESET
      if (!socket._controlReleased && !errorEmitted) {
        errorEmitted = true;
        var connReset = new Error('socket hang up');
        connReset.code = 'ECONNRESET';
        self.emit('tlsClientError', connReset, socket);
      }
    });

    socket.on('_tlsError', function(err) {
      if (!socket._controlReleased && !errorEmitted) {
        errorEmitted = true;
        self.emit('tlsClientError', err, socket);
      }
    });
  });

  if (listener) {
    this.on('secureConnection', listener);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Server.super_.prototype"></a>[module spdy.Server.super_.prototype](#apidoc.module.spdy.Server.super_.prototype)

#### <a name="apidoc.element.spdy.Server.super_.prototype.setTimeout"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.Server.super_.prototype.setTimeout)
- description and source-code
```javascript
setTimeout = function (msecs, callback) {
  this.timeout = msecs;
  if (callback)
    this.on('timeout', callback);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Server.super_.super_.prototype"></a>[module spdy.Server.super_.super_.prototype](#apidoc.module.spdy.Server.super_.super_.prototype)

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype._getServerData"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>_getServerData ()](#apidoc.element.spdy.Server.super_.super_.prototype._getServerData)
- description and source-code
```javascript
_getServerData = function () {
  return {
    ticketKeys: this.getTicketKeys().toString('hex')
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype._setServerData"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>_setServerData (data)](#apidoc.element.spdy.Server.super_.super_.prototype._setServerData)
- description and source-code
```javascript
_setServerData = function (data) {
  this.setTicketKeys(Buffer.from(data.ticketKeys, 'hex'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype.addContext"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>addContext (servername, context)](#apidoc.element.spdy.Server.super_.super_.prototype.addContext)
- description and source-code
```javascript
addContext = function (servername, context) {
  if (!servername) {
    throw new Error('"servername" is required parameter for Server.addContext');
  }

  var re = new RegExp('^' +
                      servername.replace(/([.^$+?\-\\[\]{}])/g, '\\$1')
                                .replace(/\*/g, '[^.]*') +
                      '$');
  this._contexts.push([re, tls.createSecureContext(context).context]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype.getTicketKeys"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>getTicketKeys (keys)](#apidoc.element.spdy.Server.super_.super_.prototype.getTicketKeys)
- description and source-code
```javascript
function getTicketKeys(keys) {
  return this._sharedCreds.context.getTicketKeys(keys);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype.setOptions"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>setOptions (options)](#apidoc.element.spdy.Server.super_.super_.prototype.setOptions)
- description and source-code
```javascript
setOptions = function (options) {
  if (typeof options.requestCert === 'boolean') {
    this.requestCert = options.requestCert;
  } else {
    this.requestCert = false;
  }

  if (typeof options.rejectUnauthorized === 'boolean') {
    this.rejectUnauthorized = options.rejectUnauthorized;
  } else {
    this.rejectUnauthorized = false;
  }

  if (options.pfx) this.pfx = options.pfx;
  if (options.key) this.key = options.key;
  if (options.passphrase) this.passphrase = options.passphrase;
  if (options.cert) this.cert = options.cert;
  if (options.ca) this.ca = options.ca;
  if (options.secureProtocol) this.secureProtocol = options.secureProtocol;
  if (options.crl) this.crl = options.crl;
  if (options.ciphers) this.ciphers = options.ciphers;
  if (options.ecdhCurve !== undefined)
    this.ecdhCurve = options.ecdhCurve;
  if (options.dhparam) this.dhparam = options.dhparam;
  if (options.sessionTimeout) this.sessionTimeout = options.sessionTimeout;
  if (options.ticketKeys) this.ticketKeys = options.ticketKeys;
  var secureOptions = options.secureOptions || 0;
  if (options.honorCipherOrder !== undefined)
    this.honorCipherOrder = !!options.honorCipherOrder;
  else
    this.honorCipherOrder = true;
  if (secureOptions) this.secureOptions = secureOptions;
  if (options.NPNProtocols) tls.convertNPNProtocols(options.NPNProtocols, this);
  if (options.ALPNProtocols)
    tls.convertALPNProtocols(options.ALPNProtocols, this);
  if (options.sessionIdContext) {
    this.sessionIdContext = options.sessionIdContext;
  } else {
    this.sessionIdContext = crypto.createHash('sha1')
                                  .update(process.argv.join(' '))
                                  .digest('hex')
                                  .slice(0, 32);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Server.super_.super_.prototype.setTicketKeys"></a>[function <span class="apidocSignatureSpan">spdy.Server.super_.super_.prototype.</span>setTicketKeys (keys)](#apidoc.element.spdy.Server.super_.super_.prototype.setTicketKeys)
- description and source-code
```javascript
function setTicketKeys(keys) {
  this._sharedCreds.context.setTicketKeys(keys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Socket"></a>[module spdy.Socket](#apidoc.module.spdy.Socket)

#### <a name="apidoc.element.spdy.Socket.Socket"></a>[function <span class="apidocSignatureSpan">spdy.</span>Socket (parent, options)](#apidoc.element.spdy.Socket.Socket)
- description and source-code
```javascript
function Socket(parent, options) {
  net.Socket.call(this, options);

  var state = {};

  this._spdyState = state;

  state.parent = parent;

  this.servername = parent.servername;
  this.npnProtocol = parent.npnProtocol;
  this.alpnProtocol = parent.alpnProtocol;
  this.authorized = parent.authorized;
  this.authorizationError = parent.authorizationError;
  this.encrypted = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_"></a>[function <span class="apidocSignatureSpan">spdy.Socket.</span>super_ (options)](#apidoc.element.spdy.Socket.super_)
- description and source-code
```javascript
function Socket(options) {
  if (!(this instanceof Socket)) return new Socket(options);

  this.connecting = false;
  this._hadError = false;
  this._handle = null;
  this._parent = null;
  this._host = null;

  if (typeof options === 'number')
    options = { fd: options }; // Legacy interface.
  else if (options === undefined)
    options = {};

  stream.Duplex.call(this, options);

  if (options.handle) {
    this._handle = options.handle; // private
  } else if (options.fd !== undefined) {
    this._handle = createHandle(options.fd);
    this._handle.open(options.fd);
    // options.fd can be string (since it user-defined),
    // so changing this to === would be semver-major
    // See: https://github.com/nodejs/node/pull/11513
    if ((options.fd == 1 || options.fd == 2) &&
        (this._handle instanceof Pipe) &&
        process.platform === 'win32') {
      // Make stdout and stderr blocking on Windows
      var err = this._handle.setBlocking(true);
      if (err)
        throw errnoException(err, 'setBlocking');
    }
    this.readable = options.readable !== false;
    this.writable = options.writable !== false;
  } else {
    // these will be set once there is a connection
    this.readable = this.writable = false;
  }

  // shut down the socket when we're finished with it.
  this.on('finish', onSocketFinish);
  this.on('_socketEnd', onSocketEnd);

  initSocketHandle(this);

  this._pendingData = null;
  this._pendingEncoding = '';

  // handle strings directly
  this._writableState.decodeStrings = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  // if we have a handle, then start the flow of data into the
  // buffer.  if not, then this will happen when we connect
  if (this._handle && options.readable !== false) {
    if (options.pauseOnCreate) {
      // stop the handle from reading and pause the stream
      this._handle.reading = false;
      this._handle.readStop();
      this._readableState.flowing = false;
    } else {
      this.read(0);
    }
  }

  // Reserve properties
  this.server = null;
  this._server = null;

  // Used after '.destroy()'
  this[BYTES_READ] = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Socket.prototype"></a>[module spdy.Socket.prototype](#apidoc.module.spdy.Socket.prototype)

#### <a name="apidoc.element.spdy.Socket.prototype.getCipher"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getCipher ()](#apidoc.element.spdy.Socket.prototype.getCipher)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.getEphemeralKeyInfo"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getEphemeralKeyInfo ()](#apidoc.element.spdy.Socket.prototype.getEphemeralKeyInfo)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.getPeerCertificate"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getPeerCertificate ()](#apidoc.element.spdy.Socket.prototype.getPeerCertificate)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.getSession"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getSession ()](#apidoc.element.spdy.Socket.prototype.getSession)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.getTLSTicket"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>getTLSTicket ()](#apidoc.element.spdy.Socket.prototype.getTLSTicket)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.isSessionReused"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>isSessionReused ()](#apidoc.element.spdy.Socket.prototype.isSessionReused)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.renegotiate"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>renegotiate ()](#apidoc.element.spdy.Socket.prototype.renegotiate)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.setMaxSendFragment"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setMaxSendFragment ()](#apidoc.element.spdy.Socket.prototype.setMaxSendFragment)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.setServername"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setServername ()](#apidoc.element.spdy.Socket.prototype.setServername)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.prototype.setSession"></a>[function <span class="apidocSignatureSpan">spdy.Socket.prototype.</span>setSession ()](#apidoc.element.spdy.Socket.prototype.setSession)
- description and source-code
```javascript
function methodWrap() {
  var parent = this._spdyState.parent;
  return parent[method].apply(parent, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Socket.super_"></a>[module spdy.Socket.super_](#apidoc.module.spdy.Socket.super_)

#### <a name="apidoc.element.spdy.Socket.super_.super_"></a>[function <span class="apidocSignatureSpan">spdy.Socket.</span>super_ (options)](#apidoc.element.spdy.Socket.super_.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.Socket.super_.prototype"></a>[module spdy.Socket.super_.prototype](#apidoc.module.spdy.Socket.super_.prototype)

#### <a name="apidoc.element.spdy.Socket.super_.prototype._destroy"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_destroy (exception, cb)](#apidoc.element.spdy.Socket.super_.prototype._destroy)
- description and source-code
```javascript
_destroy = function (exception, cb) {
  debug('destroy');

  function fireErrorCallbacks(self) {
    if (cb) cb(exception);
    if (exception && !self._writableState.errorEmitted) {
      process.nextTick(emitErrorNT, self, exception);
      self._writableState.errorEmitted = true;
    }
  }

  if (this.destroyed) {
    debug('already destroyed, fire error callbacks');
    fireErrorCallbacks(this);
    return;
  }

  this.connecting = false;

  this.readable = this.writable = false;

  for (var s = this; s !== null; s = s._parent)
    timers.unenroll(s);

  debug('close');
  if (this._handle) {
    if (this !== process.stderr)
      debug('close handle');
    var isException = exception ? true : false;
    // 'bytesRead' should be accessible after '.destroy()'
    this[BYTES_READ] = this._handle.bytesRead;

    this._handle.close(() => {
      debug('emit close');
      this.emit('close', isException);
    });
    this._handle.onread = noop;
    this._handle = null;
    this._sockname = null;
  }

  // we set destroyed to true before firing error callbacks in order
  // to make it re-entrance safe in case Socket.prototype.destroy()
  // is called within callbacks
  this.destroyed = true;
  fireErrorCallbacks(this);

  if (this._server) {
    ;
    debug('has server');
    this._server._connections--;
    if (this._server._emitCloseIfDrained) {
      this._server._emitCloseIfDrained();
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._getpeername"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_getpeername ()](#apidoc.element.spdy.Socket.super_.prototype._getpeername)
- description and source-code
```javascript
_getpeername = function () {
  if (!this._peername) {
    if (!this._handle || !this._handle.getpeername) {
      return {};
    }
    var out = {};
    var err = this._handle.getpeername(out);
    if (err) return {};  // FIXME(bnoordhuis) Throw?
    this._peername = out;
  }
  return this._peername;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._getsockname"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_getsockname ()](#apidoc.element.spdy.Socket.super_.prototype._getsockname)
- description and source-code
```javascript
_getsockname = function () {
  if (!this._handle || !this._handle.getsockname) {
    return {};
  }
  if (!this._sockname) {
    var out = {};
    var err = this._handle.getsockname(out);
    if (err) return {};  // FIXME(bnoordhuis) Throw?
    this._sockname = out;
  }
  return this._sockname;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._onTimeout"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_onTimeout ()](#apidoc.element.spdy.Socket.super_.prototype._onTimeout)
- description and source-code
```javascript
_onTimeout = function () {
  debug('_onTimeout');
  this.emit('timeout');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_read (n)](#apidoc.element.spdy.Socket.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  debug('_read');

  if (this.connecting || !this._handle) {
    debug('_read wait for connection');
    this.once('connect', () => this._read(n));
  } else if (!this._handle.reading) {
    // not already reading, start the flow
    debug('Socket._read readStart');
    this._handle.reading = true;
    var err = this._handle.readStart();
    if (err)
      this._destroy(errnoException(err, 'read'));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._unrefTimer"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_unrefTimer ()](#apidoc.element.spdy.Socket.super_.prototype._unrefTimer)
- description and source-code
```javascript
function _unrefTimer() {
  for (var s = this; s !== null; s = s._parent)
    timers._unrefActive(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_write (data, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype._write)
- description and source-code
```javascript
_write = function (data, encoding, cb) {
  this._writeGeneric(false, data, encoding, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._writeGeneric"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_writeGeneric (writev, data, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype._writeGeneric)
- description and source-code
```javascript
_writeGeneric = function (writev, data, encoding, cb) {
  // If we are still connecting, then buffer this for later.
  // The Writable logic will buffer up any more writes while
  // waiting for this one to be done.
  if (this.connecting) {
    this._pendingData = data;
    this._pendingEncoding = encoding;
    this.once('connect', function() {
      this._writeGeneric(writev, data, encoding, cb);
    });
    return;
  }
  this._pendingData = null;
  this._pendingEncoding = '';

  this._unrefTimer();

  if (!this._handle) {
    this._destroy(new Error('This socket is closed'), cb);
    return false;
  }

  var req = new WriteWrap();
  req.handle = this._handle;
  req.oncomplete = afterWrite;
  req.async = false;
  var err;

  if (writev) {
    var chunks = new Array(data.length << 1);
    for (var i = 0; i < data.length; i++) {
      var entry = data[i];
      chunks[i * 2] = entry.chunk;
      chunks[i * 2 + 1] = entry.encoding;
    }
    err = this._handle.writev(req, chunks);

    // Retain chunks
    if (err === 0) req._chunks = chunks;
  } else {
    var enc;
    if (data instanceof Buffer) {
      enc = 'buffer';
    } else {
      enc = encoding;
    }
    err = createWriteReq(req, this._handle, data, enc);
  }

  if (err)
    return this._destroy(errnoException(err, 'write', req.error), cb);

  this._bytesDispatched += req.bytes;

  // If it was entirely flushed, we can write some more right now.
  // However, if more is left in the queue, then wait until that clears.
  if (req.async && this._handle.writeQueueSize != 0)
    req.cb = cb;
  else
    cb();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype._writev"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>_writev (chunks, cb)](#apidoc.element.spdy.Socket.super_.prototype._writev)
- description and source-code
```javascript
_writev = function (chunks, cb) {
  this._writeGeneric(true, chunks, '', cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.address"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>address ()](#apidoc.element.spdy.Socket.super_.prototype.address)
- description and source-code
```javascript
address = function () {
  return this._getsockname();
}
```
- example usage
```shell
...
  key: "-----BEGIN RSA PRIVATE KEY-----\nMIIEpAIBAAKCAQEA4YyUIzAnCuSz43HXIPfX60XTeXJLYZZXHnyJIXdBkgE2Ou0F\nhWg0wgbicSiyCoRVQHdFcWhIYQRCq2qu3YKetRxD
/MNY9X0h0cPwf3vYP0Bqowhz\neXPc9DoUl0IwbbolYeHlchgm59w9y/UrjO8fEXxhiBpZnllR2N8C0J6p0T9Itn9y\nxN0iWOuZonrvC8upBquniDnW8X5jwTMUEMbCKBQsVoHZm7R+wfX6BfWTUDGFDh1s\norgMqFarP8TRMYqCFUfM/DFS1CeicpvN6i9SixmboIudSRXOHA+FCh0MrW+JxjDt\nBGHq3AZP0y5+f5ETQvtCWBR1xhv3fHGILshiMQIDAQABAoIBAETE5g3siprprGd2\nuE8XAkB748StsooomptzASSxBc8Mi4pf5kUMxrk5/CTgcZh/TLcBJq0zTI44DFPT\njUmAn/88hQY2UZNX+c3JXjSggAiZDWp0EzE+wGm+o7SSu81Y6jjz9U9aSdJ79mOP\ndx3bcq+UKvCiiBydwzTKmkMdfU2M2Wh/LVerXIlO5P4GsEsbenf53iafj0sHOY4W\n8mf1cWHl8/N+5Eh+0GDIIITGOjmGqNKLZOOg66wjzdY9WbCMTJUWIUjRHjCoG6ZA\nJz+vdsZQVN7M4zy8/fKkE4Vx9NEoJcDfZYa/4uo9r274TK7pJD448nTgRCKOJfMR\nCuxZHXkCgYEA5obXLtRiYXhHyXZOs/Yu9/1Iwm6zHiU66/eFRNGHzTssbPSle1kK\n/2LI3+xiRTI8PfztVP6br5/cWLKhu1ZVebCn+wJJbhpHTfAw1k1YXaCjwHh2l1OF\nPBbT4BPjK2ELNzMMF8veLY6S4yY3bQn8xUmbjQtOYuKDvFgoYAsXQo8CgYEA+nju\nhqAXSDW9yoYQBAXoduEaQH2qNfwRzY6V8rkwISI1seLPlcsd0Kc/VDOSwRdCWOk2\njn5LKPql6FfZ+9MVtPjlVLFjLcEzXttH+PkFtoA9Ffj9cxe3owNjR/tbfoHa19pV\n6+vBZJF48AlkErmVzTNlFJGWh7GtY6LgaOwdbz8CgYEAwhFaLe5WNEASDyQt9YqW\n1+a+zhBrckFdbTEfXGQYs0nRiJgch87aV01OVlSmFiLIXFcFZbxCTIOD+JfJV/DC\nXIO/pqyyLKKqzI4cTw0mCwwlTu8axyJk08VT8RxM7kPwMTQkRhQ2opuYROnzVzRF\nO8FP1lliUBTpWjHNK62qkzkCgYBZg+rLVl+7wOkpfiwvI+VmxyBYuBCi5ol+S10v\nuBuJW+6QupyxzjvDnGI3t47VT3i4yfBjkKNP6/RrSypuo4v4d5OOZy8o5Ql09y2L\nv4PZK4+pUKlT/r/0lHtg+GZEmigaSL+4ZzNgu9TbBKAtSQJOqfWQGlAQAuIS390P\n4oLKhQKBgQDiuimWRSpW3vBepzeH3SuJqm5yx/ms5RUdFH1tc/0vMZR9x/c4Ai2r\ns+1E3KacY/5z9D6t5PWaDj5Sbw8dz0zI7nvnIvufznaaGGqWlrPACQndQLnPrPSr\niFltJhhNQAMlAVOeOz75IQGuC4swdXxbdWXXPrmN9VKGPjClqU+/+w==\n-----END RSA PRIVATE KEY-----",
  cert: "-----BEGIN CERTIFICATE-----\nMIICvDCCAaagAwIBAgIDAQABMAsGCSqGSIb3DQEBDTAVMRMwEQYDVQQDFgpsb2Nh\nbC5ob3N0MB4XDTE2MDkxNzE5MDEyOVoXDTI2MDkxNjE5MDEyOVowFTETMBEGA1UE\nAxYKbG9jYWwuaG9zdDCCASAwCwYJKoZIhvcNAQEBA4IBDwAwggEKAoIBAQDhjJQj\nMCcK5LPjcdcg99frRdN5ckthllcefIkhd0GSATY67QWFaDTCBuJxKLIKhFVAd0Vx\naEhhBEKraq7dgp61HEP8w1j1fSHRw/B/e9g/QGqjCHN5c9z0OhSXQjBtuiVh4eVy\nGCbn3D3L9SuM7x8RfGGIGlmeWVHY3wLQnqnRP0i2f3LE3SJY65mieu8Ly6kGq6eI\nOdbxfmPBMxQQxsIoFCxWgdmbtH7B9foF9ZNQMYUOHWyiuAyoVqs/xNExioIVR8z8\nMVLUJ6Jym83qL1KLGZugi51JFc4cD4UKHQytb4nGMO0EYercBk/TLn5/kRNC+0JY\nFHXGG/d8cYguyGIxAgMBAAGjGzAZMBcGA1UdEQQQMA6CDCoubG9jYWwuaG9zdDAL\nBgkqhkiG9w0BAQ0DggEBAHX840Wl7APZi20i+H+eSL70/tGfld487CBnxfzvECWh\nC+mOfMH9LHSkRhkk+kyosClKO07moUev39EppR7rXhh/fDJLUAbH8Hpb8gJBu0R6\nceQQmqoHCFApqdDF0quvKq5RVatQHfTTuSNd2y/kPD6otnEfxk91rg10dpwd0jii\nv7JBV8cC+z6bDBKn46P8Hpy0k2AY8LgIpUdnmLecxcPAGh0TpGe/2FuYtvPey7vR\nKl4sqjtreZ5kbrqoKRGTU/X2bXHjhF22ZmWO/O0lv1rLrnXCnxQrSTwvXHfNsxkZ\nVqvOQufB7zDfcVrXAeQr7RpyP9qSF9aQwDQj8uio/dI=\n-----END CERTIFICATE-----"
};

const server = spdy.createServer(options, (req, res) => {
  res.end('hello');
}).listen(443, () => {
  console.log('Listening', server.address());
});
...
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.connect"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>connect (options, cb)](#apidoc.element.spdy.Socket.super_.prototype.connect)
- description and source-code
```javascript
connect = function (options, cb) {
  if (this.write !== Socket.prototype.write)
    this.write = Socket.prototype.write;

  if (options === null || typeof options !== 'object') {
    // Old API:
    // connect(port, [host], [cb])
    // connect(path, [cb]);
    var args = new Array(arguments.length);
    for (var i = 0; i < arguments.length; i++)
      args[i] = arguments[i];
    args = normalizeConnectArgs(args);
    return Socket.prototype.connect.apply(this, args);
  }

  if (this.destroyed) {
    this._readableState.reading = false;
    this._readableState.ended = false;
    this._readableState.endEmitted = false;
    this._writableState.ended = false;
    this._writableState.ending = false;
    this._writableState.finished = false;
    this._writableState.errorEmitted = false;
    this.destroyed = false;
    this._handle = null;
    this._peername = null;
    this._sockname = null;
  }

  var pipe = !!options.path;
  debug('pipe', pipe, options.path);

  if (!this._handle) {
    this._handle = pipe ? new Pipe() : new TCP();
    initSocketHandle(this);
  }

  if (typeof cb === 'function') {
    this.once('connect', cb);
  }

  this._unrefTimer();

  this.connecting = true;
  this.writable = true;

  if (pipe) {
    connect(this, options.path);
  } else {
    lookupAndConnect(this, options);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.destroy"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>destroy (exception)](#apidoc.element.spdy.Socket.super_.prototype.destroy)
- description and source-code
```javascript
destroy = function (exception) {
  debug('destroy', exception);
  this._destroy(exception);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.destroySoon"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>destroySoon ()](#apidoc.element.spdy.Socket.super_.prototype.destroySoon)
- description and source-code
```javascript
destroySoon = function () {
  if (this.writable)
    this.end();

  if (this._writableState.finished)
    this.destroy();
  else
    this.once('finish', this.destroy);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>end (data, encoding)](#apidoc.element.spdy.Socket.super_.prototype.end)
- description and source-code
```javascript
end = function (data, encoding) {
  stream.Duplex.prototype.end.call(this, data, encoding);
  this.writable = false;
  ;
  ;

  // just in case we're waiting for an EOF.
  if (this.readable && !this._readableState.endEmitted)
    this.read(0);
  else
    maybeDestroy(this);
}
```
- example usage
```shell
...
      autoSpdy31: false
    }
  }
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''

Client:
'''javascript
...
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.listen"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>listen ()](#apidoc.element.spdy.Socket.super_.prototype.listen)
- description and source-code
```javascript
listen = function () {
  debug('socket.listen');
  this.on('connection', arguments[0]);
  listen(this, null, null, null);
}
```
- example usage
```shell
...
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''

Client:
'''javascript
var spdy = require('spdy');
var http = require('http');
...
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.read"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>read (n)](#apidoc.element.spdy.Socket.super_.prototype.read)
- description and source-code
```javascript
read = function (n) {
  if (n === 0)
    return stream.Readable.prototype.read.call(this, n);

  this.read = stream.Readable.prototype.read;
  this._consuming = true;
  return this.read(n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.ref"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>ref ()](#apidoc.element.spdy.Socket.super_.prototype.ref)
- description and source-code
```javascript
ref = function () {
  if (!this._handle) {
    this.once('connect', this.ref);
    return this;
  }

  this._handle.ref();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.setKeepAlive"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setKeepAlive (setting, msecs)](#apidoc.element.spdy.Socket.super_.prototype.setKeepAlive)
- description and source-code
```javascript
setKeepAlive = function (setting, msecs) {
  if (!this._handle) {
    this.once('connect', () => this.setKeepAlive(setting, msecs));
    return this;
  }

  if (this._handle.setKeepAlive)
    this._handle.setKeepAlive(setting, ~~(msecs / 1000));

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.setNoDelay"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setNoDelay (enable)](#apidoc.element.spdy.Socket.super_.prototype.setNoDelay)
- description and source-code
```javascript
setNoDelay = function (enable) {
  if (!this._handle) {
    this.once('connect',
              enable ? this.setNoDelay : () => this.setNoDelay(enable));
    return this;
  }

  // backwards compatibility: assume true when 'enable' is omitted
  if (this._handle.setNoDelay)
    this._handle.setNoDelay(enable === undefined ? true : !!enable);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.setTimeout"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>setTimeout (msecs, callback)](#apidoc.element.spdy.Socket.super_.prototype.setTimeout)
- description and source-code
```javascript
setTimeout = function (msecs, callback) {
  if (msecs === 0) {
    timers.unenroll(this);
    if (callback) {
      this.removeListener('timeout', callback);
    }
  } else {
    timers.enroll(this, msecs);
    timers._unrefActive(this);
    if (callback) {
      this.once('timeout', callback);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.unref"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>unref ()](#apidoc.element.spdy.Socket.super_.prototype.unref)
- description and source-code
```javascript
unref = function () {
  if (!this._handle) {
    this.once('connect', this.unref);
    return this;
  }

  this._handle.unref();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.Socket.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">spdy.Socket.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.spdy.Socket.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  if (typeof chunk !== 'string' && !(chunk instanceof Buffer)) {
    throw new TypeError(
      'Invalid data, chunk must be a string or buffer, not ' + typeof chunk);
  }
  return stream.Duplex.prototype.write.apply(this, arguments);
}
```
- example usage
```shell
...
'''javascript
var req = http.request({ agent: spdyAgent, /* ... */ }).function (res) {
  // On server's trailing headers
  res.on('trailers', function(headers) {
    // ...
  });
});
req.write('stuff');
req.addTrailers({ /* ... */ });
req.end();
'''

### Options

All options supported by [tls][2] work with node-spdy.
...
```



# <a name="apidoc.module.spdy.agent"></a>[module spdy.agent](#apidoc.module.spdy.agent)

#### <a name="apidoc.element.spdy.agent.Agent"></a>[function <span class="apidocSignatureSpan">spdy.agent.</span>Agent (options)](#apidoc.element.spdy.agent.Agent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent"></a>[function <span class="apidocSignatureSpan">spdy.agent.</span>PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.create"></a>[function <span class="apidocSignatureSpan">spdy.agent.</span>create (base, options)](#apidoc.element.spdy.agent.create)
- description and source-code
```javascript
function create(base, options) {
  if (typeof base === 'object') {
    options = base;
    base = null;
  }

  if (base)
    return instantiate(base).create(options);

  if (options.spdy && options.spdy.plain)
    return exports.PlainAgent.create(options);
  else
    return exports.Agent.create(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.agent.PlainAgent"></a>[module spdy.agent.PlainAgent](#apidoc.module.spdy.agent.PlainAgent)

#### <a name="apidoc.element.spdy.agent.PlainAgent.PlainAgent"></a>[function <span class="apidocSignatureSpan">spdy.agent.</span>PlainAgent (options)](#apidoc.element.spdy.agent.PlainAgent.PlainAgent)
- description and source-code
```javascript
function Agent(options) {
  this._init(base, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.create"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.</span>create (options)](#apidoc.element.spdy.agent.PlainAgent.create)
- description and source-code
```javascript
function create(options) {
  return new Agent(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.super_"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.</span>super_ (options)](#apidoc.element.spdy.agent.PlainAgent.super_)
- description and source-code
```javascript
function Agent(options) {
  if (!(this instanceof Agent))
    return new Agent(options);

  EventEmitter.call(this);

  var self = this;

  self.defaultPort = 80;
  self.protocol = 'http:';

  self.options = util._extend({}, options);

  // don't confuse net and make it think that we're connecting to a pipe
  self.options.path = null;
  self.requests = {};
  self.sockets = {};
  self.freeSockets = {};
  self.keepAliveMsecs = self.options.keepAliveMsecs || 1000;
  self.keepAlive = self.options.keepAlive || false;
  self.maxSockets = self.options.maxSockets || Agent.defaultMaxSockets;
  self.maxFreeSockets = self.options.maxFreeSockets || 256;

  self.on('free', function(socket, options) {
    var name = self.getName(options);
    debug('agent.on(free)', name);

    if (socket.writable &&
        self.requests[name] && self.requests[name].length) {
      self.requests[name].shift().onSocket(socket);
      if (self.requests[name].length === 0) {
        // don't leak
        delete self.requests[name];
      }
    } else {
      // If there are no pending requests, then put it in
      // the freeSockets pool, but only if we're allowed to do so.
      var req = socket._httpMessage;
      if (req &&
          req.shouldKeepAlive &&
          socket.writable &&
          self.keepAlive) {
        var freeSockets = self.freeSockets[name];
        var freeLen = freeSockets ? freeSockets.length : 0;
        var count = freeLen;
        if (self.sockets[name])
          count += self.sockets[name].length;

        if (count > self.maxSockets || freeLen >= self.maxFreeSockets) {
          socket.destroy();
        } else {
          freeSockets = freeSockets || [];
          self.freeSockets[name] = freeSockets;
          socket.setKeepAlive(true, self.keepAliveMsecs);
          socket.unref();
          socket._httpMessage = null;
          self.removeSocket(socket, options);
          freeSockets.push(socket);
        }
      } else {
        socket.destroy();
      }
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.agent.PlainAgent.prototype"></a>[module spdy.agent.PlainAgent.prototype](#apidoc.module.spdy.agent.PlainAgent.prototype)

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype._connect"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_connect (options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype._connect)
- description and source-code
```javascript
function _connect(options, callback) {
  var state = this._spdyState;

  var protocols = state.options.protocols || [
    'h2',
    'spdy/3.1', 'spdy/3', 'spdy/2',
    'http/1.1', 'http/1.0'
  ];

  // TODO(indutny): reconnect automatically?
  var socket = this.createConnection(util._extend({
    NPNProtocols: protocols,
    ALPNProtocols: protocols,
    servername: options.servername || options.host
  }, options));
  state.socket = socket;

  socket.setNoDelay(true);

  function onError(err) {
    return callback(err);
  }
  socket.on('error', onError);

  socket.on(state.secure ? 'secureConnect' : 'connect', function() {
    socket.removeListener('error', onError);

    var protocol;
    if (state.secure) {
      protocol = socket.npnProtocol ||
                 socket.alpnProtocol ||
                 state.options.protocol;
    } else {
      protocol = state.options.protocol;
    }

    // HTTP server - kill socket and switch to the fallback mode
    if (!protocol || protocol === 'http/1.1' || protocol === 'http/1.0') {
      debug('activating fallback');
      socket.destroy();
      state.fallback = true;
      return;
    }

    debug('connected protocol=%j', protocol);
    var connection = transport.connection.create(socket, util._extend({
      protocol: /spdy/.test(protocol) ? 'spdy' : 'http2',
      isServer: false
    }, state.options.connection || {}));

    // Set version when we are certain
    if (protocol === 'h2') {
      connection.start(4);
    } else if (protocol === 'spdy/3.1') {
      connection.start(3.1);
    } else if (protocol === 'spdy/3') {
      connection.start(3);
    } else if (protocol === 'spdy/2') {
      connection.start(2);
    } else {
      socket.destroy();
      callback(new Error('Unexpected protocol: ' + protocol));
      return;
    }

    if (state.options['x-forwarded-for'] !== undefined)
      connection.sendXForwardedFor(state.options['x-forwarded-for']);

    callback(null, connection);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype._createSocket"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_createSocket (req, options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype._createSocket)
- description and source-code
```javascript
function _createSocket(req, options, callback) {
  var state = this._spdyState;
  if (state.fallback)
    return state.createSocket(req, options);

  var handle = spdy.handle.create(null, null, state.socket);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(state.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);
  handle.assignClientRequest(req);

  // Create stream only once 'req.end()' is called
  var self = this;
  handle.once('needStream', function() {
    if (state.connection === null) {
      self.once('_connect', function() {
        handle.setStream(self._createStream(req, handle));
      });
    } else {
      handle.setStream(self._createStream(req, handle));
    }
  });

  // Yes, it is in reverse
  req.on('response', function(res) {
    handle.assignRequest(res);
  });
  handle.assignResponse(req);

  // Handle PUSH
  req.addListener('newListener', spdy.request.onNewListener);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  if (callback)
    return callback(null, socket);

  return socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype._createStream"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_createStream (req, handle)](#apidoc.element.spdy.agent.PlainAgent.prototype._createStream)
- description and source-code
```javascript
function _createStream(req, handle) {
  var state = this._spdyState;

  var self = this;
  return state.connection.reserveStream({
    method: req.method,
    path: req.path,
    headers: req._headers,
    host: state.host
  }, function(err, stream) {
    if (err)
      return self.emit('error', err);

    stream.on('response', function(status, headers) {
      handle.emitResponse(status, headers);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype._getCreateSocket"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_getCreateSocket ()](#apidoc.element.spdy.agent.PlainAgent.prototype._getCreateSocket)
- description and source-code
```javascript
function _getCreateSocket() {
  // Find super's 'createSocket' method
  var createSocket;
  var cons = this.constructor.super_;
  do {
    createSocket = cons.prototype.createSocket;

    if (cons.super_ === EventEmitter || !cons.super_)
      break;
    cons = cons.super_;
  } while (!createSocket);
  if (!createSocket)
    createSocket = http.Agent.prototype.createSocket;

  assert(createSocket, '.createSocket() method not found');

  return createSocket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype._init"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>_init (base, options)](#apidoc.element.spdy.agent.PlainAgent.prototype._init)
- description and source-code
```javascript
function _init(base, options) {
  base.call(this, options);

  var state = {};
  this._spdyState = state;

  state.host = options.host;
  state.options = options.spdy || {};
  state.secure = this instanceof https.Agent;
  state.fallback = false;
  state.createSocket = this._getCreateSocket();
  state.socket = null;
  state.connection = null;

  // No chunked encoding
  this.keepAlive = false;

  var self = this;
  this._connect(options, function(err, connection) {
    if (err)
      return self.emit('error', err);

    state.connection = connection;
    self.emit('_connect');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype.close"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>close (callback)](#apidoc.element.spdy.agent.PlainAgent.prototype.close)
- description and source-code
```javascript
function close(callback) {
  var state = this._spdyState;

  if (state.connection === null) {
    this.once('_connect', function() {
      this.close(callback);
    });
    return;
  }

  state.connection.end(callback);
}
```
- example usage
```shell
...
  agent: agent
}, function(response) {
  console.log('yikes');
  // Here it goes like with any other node.js HTTP request
  // ...
  // And once we're done - we may close TCP connection to server
  // NOTE: All non-closed requests will die!
  agent.close();
}).end();
'''

Please note that if you use a custom agent, by default all connection-level
errors will result in an uncaught exception. To handle these errors subscribe
to the 'error' event and re-emit the captured error:
...
```

#### <a name="apidoc.element.spdy.agent.PlainAgent.prototype.createSocket"></a>[function <span class="apidocSignatureSpan">spdy.agent.PlainAgent.prototype.</span>createSocket (req, options, callback)](#apidoc.element.spdy.agent.PlainAgent.prototype.createSocket)
- description and source-code
```javascript
function _createSocket(req, options, callback) {
  var state = this._spdyState;
  if (state.fallback)
    return state.createSocket(req, options);

  var handle = spdy.handle.create(null, null, state.socket);

  var socketOptions = {
    handle: handle,
    allowHalfOpen: true
  };

  var socket;
  if (state.secure)
    socket = new spdy.Socket(state.socket, socketOptions);
  else
    socket = new net.Socket(socketOptions);

  handle.assignSocket(socket);
  handle.assignClientRequest(req);

  // Create stream only once 'req.end()' is called
  var self = this;
  handle.once('needStream', function() {
    if (state.connection === null) {
      self.once('_connect', function() {
        handle.setStream(self._createStream(req, handle));
      });
    } else {
      handle.setStream(self._createStream(req, handle));
    }
  });

  // Yes, it is in reverse
  req.on('response', function(res) {
    handle.assignRequest(res);
  });
  handle.assignResponse(req);

  // Handle PUSH
  req.addListener('newListener', spdy.request.onNewListener);

  // For v0.8
  socket.readable = true;
  socket.writable = true;

  if (callback)
    return callback(null, socket);

  return socket;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.handle"></a>[module spdy.handle](#apidoc.module.spdy.handle)

#### <a name="apidoc.element.spdy.handle.handle"></a>[function <span class="apidocSignatureSpan">spdy.</span>handle (options, stream, socket)](#apidoc.element.spdy.handle.handle)
- description and source-code
```javascript
function Handle(options, stream, socket) {
  var state = {};
  this._spdyState = state;

  state.options = options || {};

  state.stream = stream;
  state.socket = null;
  state.rawSocket = socket || stream.connection.socket;
  state.deceiver = null;
  state.ending = false;

  var self = this;
  thing.call(this, stream, {
    getPeerName: function() {
      return self._getPeerName();
    },
    close: function(callback) {
      return self._closeCallback(callback);
    }
  });

  if (!state.stream) {
    this.on('stream', function(stream) {
      state.stream = stream;
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.create"></a>[function <span class="apidocSignatureSpan">spdy.handle.</span>create (options, stream, socket)](#apidoc.element.spdy.handle.create)
- description and source-code
```javascript
function create(options, stream, socket) {
  return new Handle(options, stream, socket);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_"></a>[function <span class="apidocSignatureSpan">spdy.handle.</span>super_ (stream, options)](#apidoc.element.spdy.handle.super_)
- description and source-code
```javascript
function Handle(stream, options) {
  EventEmitter.call(this);

  this._stream = stream;
  this._flowing = false;
  this._reading = false;
  this._options = options || {};

  this.onread = null;

  // Pending requests
  this.pending = new Queue();

  // Start handle once 'onread' is set
  if (mode === 'rusty') {
    var self = this;
    Object.defineProperty(this, 'onread', {
      set: function(value) {
        Object.defineProperty(self, 'onread', {
          value: value
        });
        process.nextTick(function() {
          self.readStart();
        });
      }
    });
  }

  // NOTE: v0.8 has some odd .pause()/.resume() semantics in http.js
  if (mode === 'rusty')
    this.writeQueueSize = 0;
  else if (mode !== 'modern')
    this.writeQueueSize = 1;

  if (mode === 'rusty') {
    if (this._stream)
      this._rustyInit();
    else
      this.once('stream', this._rustyInit);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.handle.prototype"></a>[module spdy.handle.prototype](#apidoc.module.spdy.handle.prototype)

#### <a name="apidoc.element.spdy.handle.prototype._closeCallback"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_closeCallback (callback)](#apidoc.element.spdy.handle.prototype._closeCallback)
- description and source-code
```javascript
function _closeCallback(callback) {
  var state = this._spdyState;
  var stream = state.stream;

  if (state.ending) {
    // The .end() method of the stream may be called by us or by the
    // .shutdown() method in our super-class. If the latter has already been
    // called, then calling the .end() method below will have no effect, with
    // the result that the callback will never get executed, leading to an ever
    // so subtle memory leak.
    if (stream._writableState.finished) {
      // NOTE: it is important to call 'setImmediate' instead of 'nextTick',
      // since this is how regular 'handle.close()' works in node.js core.
      //
      // Using 'nextTick' will lead to 'net.Socket' emitting 'close' before
      // 'end' on UV_EOF. This results in aborted request without 'end' event.
      setImmediate(callback);
    } else if (stream._writableState.ending) {
      stream.once('finish', function() {
        callback(null);
      });
    } else {
      stream.end(callback);
    }
  } else {
    stream.abort(callback);
  }

  // Only a single end is allowed
  state.ending = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype._getPeerName"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_getPeerName ()](#apidoc.element.spdy.handle.prototype._getPeerName)
- description and source-code
```javascript
function _getPeerName() {
  var state = this._spdyState;

  if (state.rawSocket._getpeername)
    return state.rawSocket._getpeername();

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype._transformHeaders"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>_transformHeaders (kind, headers)](#apidoc.element.spdy.handle.prototype._transformHeaders)
- description and source-code
```javascript
function _transformHeaders(kind, headers) {
  var state = this._spdyState;

  var res = {};
  var keys = Object.keys(headers);

  if (kind === 'request' && state.options['x-forwarded-for']) {
    var xforwarded = state.stream.connection.getXForwardedFor();
    if (xforwarded !== null)
      res['x-forwarded-for'] = xforwarded;
  }

  for (var i = 0; i < keys.length; i++) {
    var key = keys[i];
    var value = headers[key];

    if (key === ':authority')
      res.host = value;
    if (/^:/.test(key))
      continue;

    res[key] = value;
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.assignClientRequest"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignClientRequest (req)](#apidoc.element.spdy.handle.prototype.assignClientRequest)
- description and source-code
```javascript
function assignClientRequest(req) {
  var state = this._spdyState;
  var oldEnd = req.end;
  var oldSend = req._send;

  // Catch the headers before request will be sent
  var self = this;

  // For old nodes
  if (thing.mode !== 'modern') {
    req.end = function end() {
      this.end = oldEnd;

      this._send('');

      return this.end.apply(this, arguments);
    };
  }

  req._send = function send(data) {
    this._headerSent = true;

    // for v0.10 and below, otherwise it will set 'hot = false' and include
    // headers in first write
    this._header = 'ignore me';

    // To prevent exception
    this.connection = state.socket;

    // It is very important to leave this here, otherwise it will be executed
    // on a next tick, after '_send' will perform write
    self.getStream(function(stream) {
      stream.send();
    });

    // We are ready to create stream
    self.emit('needStream');

    req._send = oldSend;

    // Ignore empty writes
    if (req.method === 'GET' && data.length === 0)
      return;

    return req._send.apply(this, arguments);
  };

  // No chunked encoding
  req.useChunkedEncodingByDefault = false;

  req.on('finish', function() {
    req.socket.end();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.assignRequest"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignRequest (req)](#apidoc.element.spdy.handle.prototype.assignRequest)
- description and source-code
```javascript
function assignRequest(req) {
  // Emit trailing headers
  this.getStream(function(stream) {
    stream.on('headers', function(headers) {
      req.emit('trailers', headers);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.assignResponse"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignResponse (res)](#apidoc.element.spdy.handle.prototype.assignResponse)
- description and source-code
```javascript
function assignResponse(res) {
  var self = this;

  res.addTrailers = function addTrailers(headers) {
    self.getStream(function(stream) {
      stream.sendHeaders(headers);
    });
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.assignSocket"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>assignSocket (socket, options)](#apidoc.element.spdy.handle.prototype.assignSocket)
- description and source-code
```javascript
function assignSocket(socket, options) {
  var state = this._spdyState;

  state.socket = socket;
  state.deceiver = httpDeceiver.create(socket, options);

  function onStreamError(err) {
    state.socket.emit('error', err);
  }

  this.getStream(function(stream) {
    stream.on('error', onStreamError);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.emitRequest"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>emitRequest ()](#apidoc.element.spdy.handle.prototype.emitRequest)
- description and source-code
```javascript
function emitRequest() {
  var state = this._spdyState;
  var stream = state.stream;

  state.deceiver.emitRequest({
    method: stream.method,
    path: stream.path,
    headers: this._transformHeaders('request', stream.headers)
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.emitResponse"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>emitResponse (status, headers)](#apidoc.element.spdy.handle.prototype.emitResponse)
- description and source-code
```javascript
function emitResponse(status, headers) {
  var state = this._spdyState;

  state.deceiver.emitResponse({
    status: status,
    headers: this._transformHeaders('response', headers)
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.prototype.getStream"></a>[function <span class="apidocSignatureSpan">spdy.handle.prototype.</span>getStream (callback)](#apidoc.element.spdy.handle.prototype.getStream)
- description and source-code
```javascript
function getStream(callback) {
  var state = this._spdyState;

  if (!callback) {
    assert(state.stream);
    return state.stream;
  }

  if (state.stream) {
    process.nextTick(function() {
      callback(state.stream);
    });
    return;
  }

  this.on('stream', callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.handle.super_"></a>[module spdy.handle.super_](#apidoc.module.spdy.handle.super_)

#### <a name="apidoc.element.spdy.handle.super_.super_"></a>[function <span class="apidocSignatureSpan">spdy.handle.</span>super_ ()](#apidoc.element.spdy.handle.super_.super_)
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

#### <a name="apidoc.element.spdy.handle.super_.create"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.</span>create (stream, options)](#apidoc.element.spdy.handle.super_.create)
- description and source-code
```javascript
function create(stream, options) {
  return new Handle(stream, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.handle.super_.prototype"></a>[module spdy.handle.super_.prototype](#apidoc.module.spdy.handle.super_.prototype)

#### <a name="apidoc.element.spdy.handle.super_.prototype._close"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_close ()](#apidoc.element.spdy.handle.super_.prototype._close)
- description and source-code
```javascript
function _close() {
  var list = this._pendingList();

  var self = this;
  setImmediate(function() {
    for (var i = 0; i < list.length; i++) {
      var req = list[i];
      req.oncomplete(uv.UV_ECANCELED, self, req);
    }
  });

  this.readStop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype._flow"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_flow ()](#apidoc.element.spdy.handle.super_.prototype._flow)
- description and source-code
```javascript
function flow() {
  var self = this;
  this._stream.on('data', function(chunk) {
    self.onread(chunk.length, chunk);
  });

  this._stream.on('end', function() {
    self.onread(uv.UV_EOF, new Buffer(0));
  });

  this._stream.on('close', function() {
    setImmediate(function() {
      if (self._reading)
        self.onread(uv.UV_ECONNRESET, new Buffer(0));
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype._pendingList"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_pendingList ()](#apidoc.element.spdy.handle.super_.prototype._pendingList)
- description and source-code
```javascript
function _pendingList() {
  var list = [];
  while (!this.pending.isEmpty())
    list.push(this.pending.first().dequeue());
  return list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype._queueReq"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_queueReq (type, req)](#apidoc.element.spdy.handle.super_.prototype._queueReq)
- description and source-code
```javascript
function _queueReq(type, req) {
  return this.pending.append(type, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype._shutdown"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_shutdown (wrap)](#apidoc.element.spdy.handle.super_.prototype._shutdown)
- description and source-code
```javascript
function _shutdown(wrap) {
  var self = this;
  this._stream.end(function() {
    var req = wrap.dequeue();
    if (!req)
      return;

    req.oncomplete(0, self, req);
  });
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype._writeEnc"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>_writeEnc (wrap, req, data, enc)](#apidoc.element.spdy.handle.super_.prototype._writeEnc)
- description and source-code
```javascript
function _writeEnc(wrap, req, data, enc) {
  var self = this;

  req.async = true;
  req.bytes = data.length;

  if (wrap.isEmpty())
    return 0;

  this._stream.write(data, enc, function() {
    var req = wrap.dequeue();
    if (!req)
      return;
    req.oncomplete(0, self, req);
  });

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>close (callback)](#apidoc.element.spdy.handle.super_.prototype.close)
- description and source-code
```javascript
function close(callback) {
  this._close();

  if (!this._stream) {
    this.once('stream', function() {
      this.close(callback);
    });
    return 0;
  }

  if (this._options.close)
    this._options.close(callback);
  else
    process.nextTick(callback);

  return 0;
}
```
- example usage
```shell
...
  agent: agent
}, function(response) {
  console.log('yikes');
  // Here it goes like with any other node.js HTTP request
  // ...
  // And once we're done - we may close TCP connection to server
  // NOTE: All non-closed requests will die!
  agent.close();
}).end();
'''

Please note that if you use a custom agent, by default all connection-level
errors will result in an uncaught exception. To handle these errors subscribe
to the 'error' event and re-emit the captured error:
...
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.getpeername"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>getpeername (out)](#apidoc.element.spdy.handle.super_.prototype.getpeername)
- description and source-code
```javascript
function getpeername(out) {
  var res = this.getsockname();
  if (!res)
    return -1;

  Object.keys(res).forEach(function(key) {
    out[key] = res[key];
  });

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.getsockname"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>getsockname ()](#apidoc.element.spdy.handle.super_.prototype.getsockname)
- description and source-code
```javascript
function getsockname() {
  if (this._options.getPeerName)
    return this._options.getPeerName();
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.readStart"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>readStart ()](#apidoc.element.spdy.handle.super_.prototype.readStart)
- description and source-code
```javascript
function readStart() {
  this._reading = true;

  if (!this._stream) {
    this.once('stream', this.readStart);
    return 0;
  }

  if (!this._flowing) {
    this._flowing = true;
    this._flow();
  }

  this._stream.resume();
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.readStop"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>readStop ()](#apidoc.element.spdy.handle.super_.prototype.readStop)
- description and source-code
```javascript
function readStop() {
  this._reading = false;

  if (!this._stream) {
    this.once('stream', this.readStop);
    return 0;
  }
  this._stream.pause();
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.setStream"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>setStream (stream)](#apidoc.element.spdy.handle.super_.prototype.setStream)
- description and source-code
```javascript
function setStream(stream) {
  assert(this._stream === null, 'Can\'t set stream two times');
  this._stream = stream;

  this.emit('stream', stream);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.shutdown"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>shutdown (req)](#apidoc.element.spdy.handle.super_.prototype.shutdown)
- description and source-code
```javascript
function shutdown(req) {
  var wrap = this._queueReq('shutdown', req);

  if (!this._stream) {
    this.once('stream', function() {
      this._shutdown(wrap);
    });
    return 0;
  }

  return this._shutdown(wrap);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeAsciiString"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeAsciiString (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeAsciiString)
- description and source-code
```javascript
function writeAsciiString(req, data) {
  return this.writeEnc(req, data, 'ascii');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeBinaryString"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeBinaryString (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeBinaryString)
- description and source-code
```javascript
function writeBinaryString(req, data) {
  return this.writeEnc(req, data, 'binary');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeBuffer"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeBuffer (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeBuffer)
- description and source-code
```javascript
function writeBuffer(req, data) {
  return this.writeEnc(req, data, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeEnc"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeEnc (req, data, enc)](#apidoc.element.spdy.handle.super_.prototype.writeEnc)
- description and source-code
```javascript
function writeEnc(req, data, enc) {
  var wrap = this._queueReq('write', req);

  if (!this._stream) {
    this.once('stream', function() {
      this._writeEnc(wrap, req, data, enc);
    });

    return 0;
  }

  return this._writeEnc(wrap, req, data, enc);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeLatin1String"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeLatin1String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeLatin1String)
- description and source-code
```javascript
function writeLatin1String(req, data) {
  return this.writeEnc(req, data, 'binary');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeUcs2String"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeUcs2String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeUcs2String)
- description and source-code
```javascript
function writeUcs2String(req, data) {
  return this.writeEnc(req, data, 'ucs2');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.handle.super_.prototype.writeUtf8String"></a>[function <span class="apidocSignatureSpan">spdy.handle.super_.prototype.</span>writeUtf8String (req, data)](#apidoc.element.spdy.handle.super_.prototype.writeUtf8String)
- description and source-code
```javascript
function writeUtf8String(req, data) {
  return this.writeEnc(req, data, 'utf8');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.request"></a>[module spdy.request](#apidoc.module.spdy.request)

#### <a name="apidoc.element.spdy.request.onNewListener"></a>[function <span class="apidocSignatureSpan">spdy.request.</span>onNewListener (type)](#apidoc.element.spdy.request.onNewListener)
- description and source-code
```javascript
function onNewListener(type) {
  var req = this;

  if (type !== 'push')
    return;

  // Not first listener
  if (req.listeners('push').length !== 0)
    return;

  if (!req.socket) {
    req.on('socket', function() {
      attachPush(req);
    });
    return;
  }

  attachPush(req);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spdy.response"></a>[module spdy.response](#apidoc.module.spdy.response)

#### <a name="apidoc.element.spdy.response.end"></a>[function <span class="apidocSignatureSpan">spdy.response.</span>end (data, encoding, callback)](#apidoc.element.spdy.response.end)
- description and source-code
```javascript
function end(data, encoding, callback) {
  if (!this._headerSent)
    this.writeHead(this.statusCode);

  if (!this.socket._handle)
    return;

  // Compatibility with Node.js core
  this.finished = true;

  var self = this;
  var handle = this.socket._handle;
  handle._spdyState.ending = true;
  this.socket.end(data, encoding, function() {
    self.constructor.prototype.end.call(self, '', 'utf8', callback);
  });
}
```
- example usage
```shell
...
      autoSpdy31: false
    }
  }
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''

Client:
'''javascript
...
```

#### <a name="apidoc.element.spdy.response.push"></a>[function <span class="apidocSignatureSpan">spdy.response.</span>push (path, headers, callback)](#apidoc.element.spdy.response.push)
- description and source-code
```javascript
function push(path, headers, callback) {
  var frame = {
    path: path,
    method: headers.method ? headers.method.toString() : 'GET',
    status: headers.status ? parseInt(headers.status, 10) : 200,
    host: this._req.headers.host,
    headers: headers.request,
    response: headers.response
  };

  var stream = this.spdyStream;
  return stream.pushPromise(frame, callback);
}
```
- example usage
```shell
...
### Push streams

It is possible to initiate [PUSH_PROMISE][5] to send content to clients _before_
the client requests it.

'''javascript
spdy.createServer(options, function(req, res) {
var stream = res.push('/main.js', {
  status: 200, // optional
  method: 'GET', // optional
  request: {
    accept: '*/*'
  },
  response: {
    'content-type': 'application/javascript'
...
```

#### <a name="apidoc.element.spdy.response.writeContinue"></a>[function <span class="apidocSignatureSpan">spdy.response.</span>writeContinue (callback)](#apidoc.element.spdy.response.writeContinue)
- description and source-code
```javascript
function writeContinue(callback) {
  if (this.socket._handle)
    this.socket._handle._spdyState.stream.respond(100, {}, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.response.writeHead"></a>[function <span class="apidocSignatureSpan">spdy.response.</span>writeHead (statusCode, reason, obj)](#apidoc.element.spdy.response.writeHead)
- description and source-code
```javascript
function writeHead(statusCode, reason, obj) {
  var headers;

  if (typeof reason === 'string') {
    // writeHead(statusCode, reasonPhrase[, headers])
    this.statusMessage = reason;
  } else {
    // writeHead(statusCode[, headers])
    this.statusMessage =
      this.statusMessage || 'unknown';
    obj = reason;
  }
  this.statusCode = statusCode;

  if (this._headers) {
    // Slow-case: when progressive API and header fields are passed.
    if (obj) {
      var keys = Object.keys(obj);
      for (var i = 0; i < keys.length; i++) {
        var k = keys[i];
        if (k) this.setHeader(k, obj[k]);
      }
    }
    // only progressive api is used
    headers = this._renderHeaders();
  } else {
    // only writeHead() called
    headers = obj;
  }

  if (statusCode === 204 || statusCode === 304 ||
      (100 <= statusCode && statusCode <= 199)) {
    // RFC 2616, 10.2.5:
    // The 204 response MUST NOT include a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    // RFC 2616, 10.3.5:
    // The 304 response MUST NOT contain a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    // RFC 2616, 10.1 Informational 1xx:
    // This class of status code indicates a provisional response,
    // consisting only of the Status-Line and optional headers, and is
    // terminated by an empty line.
    this._hasBody = false;
  }

  // don't keep alive connections where the client expects 100 Continue
  // but we sent a final status; they may put extra bytes on the wire.
  if (this._expect_continue && !this._sent100) {
    this.shouldKeepAlive = false;
  }

  // Implicit headers sent!
  this._header = true;
  this._headerSent = true;

  if (this.socket._handle)
    this.socket._handle._spdyState.stream.respond(this.statusCode, headers);
}
```
- example usage
```shell
...
      // **optional** if true - server will send 3.1 frames on 3.0 *plain* spdy
      autoSpdy31: false
    }
  }
};

var server = spdy.createServer(options, function(req, res) {
  res.writeHead(200);
  res.end('hello world!');
});

server.listen(3000);
'''

Client:
...
```



# <a name="apidoc.module.spdy.server"></a>[module spdy.server](#apidoc.module.spdy.server)

#### <a name="apidoc.element.spdy.server.PlainServer"></a>[function <span class="apidocSignatureSpan">spdy.server.</span>PlainServer (options, handler)](#apidoc.element.spdy.server.PlainServer)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.server.Server"></a>[function <span class="apidocSignatureSpan">spdy.server.</span>Server (options, handler)](#apidoc.element.spdy.server.Server)
- description and source-code
```javascript
function Server(options, handler) {
  this._init(base, options, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spdy.server.create"></a>[function <span class="apidocSignatureSpan">spdy.server.</span>create (base, options, handler)](#apidoc.element.spdy.server.create)
- description and source-code
```javascript
function create(base, options, handler) {
  if (typeof base === 'object') {
    handler = options;
    options = base;
    base = null;
  }

  if (base)
    return instantiate(base).create(options, handler);

  if (options.spdy && options.spdy.plain)
    return exports.PlainServer.create(options, handler);
  else
    return exports.Server.create(options, handler);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
