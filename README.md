# api documentation for  [wordpress (v1.4.0)](https://github.com/scottgonzalez/node-wordpress)  [![npm package](https://img.shields.io/npm/v/npmdoc-wordpress.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-wordpress) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-wordpress.svg)](https://travis-ci.org/npmdoc/node-npmdoc-wordpress)
#### A client for working with WordPress.

[![NPM](https://nodei.co/npm/wordpress.png?downloads=true)](https://www.npmjs.com/package/wordpress)

[![apidoc](https://npmdoc.github.io/node-npmdoc-wordpress/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-wordpress_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-wordpress/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-wordpress/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-wordpress/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Scott González",
        "email": "scott.gonzalez@gmail.com",
        "url": "http://scottgonzalez.com"
    },
    "bugs": {
        "url": "https://github.com/scottgonzalez/node-wordpress/issues"
    },
    "dependencies": {
        "xmlrpc": "1.3.2"
    },
    "description": "A client for working with WordPress.",
    "devDependencies": {
        "jshint": "2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "036e0f5a0e880409dcad3022364de8b67efdc348",
        "tarball": "https://registry.npmjs.org/wordpress/-/wordpress-1.4.0.tgz"
    },
    "gitHead": "fbd8cdb0d6e9d35c2a40979866d0b20633f5e98b",
    "homepage": "https://github.com/scottgonzalez/node-wordpress",
    "license": "MIT",
    "main": "lib/wordpress.js",
    "maintainers": [
        {
            "name": "scott.gonzalez",
            "email": "scott.gonzalez@gmail.com"
        }
    ],
    "name": "wordpress",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/scottgonzalez/node-wordpress.git"
    },
    "scripts": {
        "test": "jshint lib/*"
    },
    "version": "1.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module wordpress](#apidoc.module.wordpress)
1.  [function <span class="apidocSignatureSpan">wordpress.</span>Client ( settings )](#apidoc.element.wordpress.Client)
1.  [function <span class="apidocSignatureSpan">wordpress.</span>createClient ( settings )](#apidoc.element.wordpress.createClient)
1.  object <span class="apidocSignatureSpan">wordpress.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">wordpress.</span>fieldMap

#### [module wordpress.Client](#apidoc.module.wordpress.Client)
1.  [function <span class="apidocSignatureSpan">wordpress.</span>Client ( settings )](#apidoc.element.wordpress.Client.Client)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.</span>parseUrl ( wpUrl )](#apidoc.element.wordpress.Client.parseUrl)

#### [module wordpress.Client.prototype](#apidoc.module.wordpress.Client.prototype)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>authenticatedCall ()](#apidoc.element.wordpress.Client.prototype.authenticatedCall)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>call ( method )](#apidoc.element.wordpress.Client.prototype.call)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>deletePost ( id, fn )](#apidoc.element.wordpress.Client.prototype.deletePost)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>deleteTerm ( taxonomy, id, fn )](#apidoc.element.wordpress.Client.prototype.deleteTerm)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>editPost ( id, data, fn )](#apidoc.element.wordpress.Client.prototype.editPost)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>editTerm ( id, data, fn )](#apidoc.element.wordpress.Client.prototype.editTerm)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getMediaItem ( id, fn )](#apidoc.element.wordpress.Client.prototype.getMediaItem)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getMediaLibrary ( filter, fn )](#apidoc.element.wordpress.Client.prototype.getMediaLibrary)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPost ( id, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPost)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPostType ( name, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPostType)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPostTypes ( filter, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPostTypes)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPosts ( filter, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPosts)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTaxonomies ( fn )](#apidoc.element.wordpress.Client.prototype.getTaxonomies)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTaxonomy ( name, fn )](#apidoc.element.wordpress.Client.prototype.getTaxonomy)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTerm ( taxonomy, id, fn )](#apidoc.element.wordpress.Client.prototype.getTerm)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTerms ( taxonomy, filter, fn )](#apidoc.element.wordpress.Client.prototype.getTerms)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>listMethods ( fn )](#apidoc.element.wordpress.Client.prototype.listMethods)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>newPost ( data, fn )](#apidoc.element.wordpress.Client.prototype.newPost)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>newTerm ( data, fn )](#apidoc.element.wordpress.Client.prototype.newTerm)
1.  [function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>uploadFile ( data, fn )](#apidoc.element.wordpress.Client.prototype.uploadFile)

#### [module wordpress.fieldMap](#apidoc.module.wordpress.fieldMap)
1.  [function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>array ( data, type )](#apidoc.element.wordpress.fieldMap.array)
1.  [function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>from ( data, type )](#apidoc.element.wordpress.fieldMap.from)
1.  [function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>to ( data, type )](#apidoc.element.wordpress.fieldMap.to)



# <a name="apidoc.module.wordpress"></a>[module wordpress](#apidoc.module.wordpress)

#### <a name="apidoc.element.wordpress.Client"></a>[function <span class="apidocSignatureSpan">wordpress.</span>Client ( settings )](#apidoc.element.wordpress.Client)
- description and source-code
```javascript
function Client( settings ) {
	[ "url", "username", "password" ].forEach(function( prop ) {
		if ( !settings.hasOwnProperty( prop ) ) {
			throw new Error( "Missing required setting: " + prop );
		}
	});

	var parsedUrl = Client.parseUrl( settings.url );
	this.rpc = xmlrpc[ parsedUrl.secure ? "createSecureClient" : "createClient" ]({
		host: settings.host || parsedUrl.host,
		port: parsedUrl.port,
		path: parsedUrl.path,
		rejectUnauthorized: settings.rejectUnauthorized !== undefined ? settings.rejectUnauthorized : true,

		// Always set Host header in case we're pointing to a different server
		// via settings.host
		headers: {
			Host: parsedUrl.host
		},
		basic_auth: !settings.basicAuth ? null : {
			user: settings.basicAuth.username,
			pass: settings.basicAuth.password
		}
	});
	this.blogId = settings.blogId || 0;
	this.username = settings.username;
	this.password = settings.password;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wordpress.createClient"></a>[function <span class="apidocSignatureSpan">wordpress.</span>createClient ( settings )](#apidoc.element.wordpress.createClient)
- description and source-code
```javascript
createClient = function ( settings ) {
		return new Client( settings );
	}
```
- example usage
```shell
...



## Usage

'''js
var wordpress = require( "wordpress" );
var client = wordpress.createClient({
	url: "my-site.com",
	username: "admin",
	password: "secret"
});

client.getPosts(function( error, posts ) {
	console.log( "Found " + posts.length + " posts!" );
...
```



# <a name="apidoc.module.wordpress.Client"></a>[module wordpress.Client](#apidoc.module.wordpress.Client)

#### <a name="apidoc.element.wordpress.Client.Client"></a>[function <span class="apidocSignatureSpan">wordpress.</span>Client ( settings )](#apidoc.element.wordpress.Client.Client)
- description and source-code
```javascript
function Client( settings ) {
	[ "url", "username", "password" ].forEach(function( prop ) {
		if ( !settings.hasOwnProperty( prop ) ) {
			throw new Error( "Missing required setting: " + prop );
		}
	});

	var parsedUrl = Client.parseUrl( settings.url );
	this.rpc = xmlrpc[ parsedUrl.secure ? "createSecureClient" : "createClient" ]({
		host: settings.host || parsedUrl.host,
		port: parsedUrl.port,
		path: parsedUrl.path,
		rejectUnauthorized: settings.rejectUnauthorized !== undefined ? settings.rejectUnauthorized : true,

		// Always set Host header in case we're pointing to a different server
		// via settings.host
		headers: {
			Host: parsedUrl.host
		},
		basic_auth: !settings.basicAuth ? null : {
			user: settings.basicAuth.username,
			pass: settings.basicAuth.password
		}
	});
	this.blogId = settings.blogId || 0;
	this.username = settings.username;
	this.password = settings.password;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wordpress.Client.parseUrl"></a>[function <span class="apidocSignatureSpan">wordpress.Client.</span>parseUrl ( wpUrl )](#apidoc.element.wordpress.Client.parseUrl)
- description and source-code
```javascript
parseUrl = function ( wpUrl ) {
	var urlParts, secure;

	// allow URLs without a protocol
	if ( !(/\w+:\/\//.test( wpUrl ) ) ) {
		wpUrl = "http://" + wpUrl;
	}
	urlParts = url.parse( wpUrl );
	secure = urlParts.protocol === "https:";

	return {
		host: urlParts.hostname,
		port: urlParts.port || (secure ? 443 : 80),
		path: urlParts.path.replace( /\/+$/, "" ) + "/xmlrpc.php",
		secure: secure
	};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.wordpress.Client.prototype"></a>[module wordpress.Client.prototype](#apidoc.module.wordpress.Client.prototype)

#### <a name="apidoc.element.wordpress.Client.prototype.authenticatedCall"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>authenticatedCall ()](#apidoc.element.wordpress.Client.prototype.authenticatedCall)
- description and source-code
```javascript
authenticatedCall = function () {
		var args = [].slice.call( arguments );
		args.splice( 1, 0, this.blogId, this.username, this.password );
		this.call.apply( this, args );
	}
```
- example usage
```shell
...
Invokes a method.

* 'method': The method to call.
* 'args' (optional): Arguments to pass to the method.
* 'callback' ('function( error [, data] )'): A callback to invoke when the API call is complete.
  * 'data': Data returned by the method.

#### client.authenticatedCall( method [, args... ], callback )

Invokes a method with the username and password provided by the client.

* 'method': The method to call.
* 'args' (optional): Arguments to pass to the method.
* 'callback' ('function( error [, data] )'): A callback to invoke when the API call is complete.
* 'data': Data returned by the method.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.call"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>call ( method )](#apidoc.element.wordpress.Client.prototype.call)
- description and source-code
```javascript
call = function ( method ) {
		var args = parseArguments( arguments ),
			fn = args.pop();

		if ( typeof fn !== "function" ) {
			args.push( fn );
			fn = null;
		}

		this.rpc.methodCall( method, args, function( error, data ) {
			if ( !error ) {
				return fn( null, data );
			}

			if ( error.code === "ENOTFOUND" && error.syscall === "getaddrinfo" ) {
				error.message = "Unable to connect to WordPress.";
			} else if ( error.message === "Unknown XML-RPC tag 'TITLE'" ) {
				var additional = error.res.statusCode;
				if (error.res.statusMessage) {
					additional += "; " + error.res.statusMessage;
				}

				error.message = "(" + additional + ") " + error.message;
			}

			fn( error );
		});
	}
```
- example usage
```shell
...
#### client.listMethods( callback )

Gets a list of all avaialble methods.

* 'callback' ('function( error, methods )'): A callback to invoke when the API call is complete.
* 'methods': An array of methods.

#### client.call( method [, args... ], callback )

Invokes a method.

* 'method': The method to call.
* 'args' (optional): Arguments to pass to the method.
* 'callback' ('function( error [, data] )'): A callback to invoke when the API call is complete.
* 'data': Data returned by the method.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.deletePost"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>deletePost ( id, fn )](#apidoc.element.wordpress.Client.prototype.deletePost)
- description and source-code
```javascript
deletePost = function ( id, fn ) {
		this.authenticatedCall( "wp.deletePost", id, fn );
	}
```
- example usage
```shell
...

Edits an existing post.

* 'id': The ID of the post to edit.
* 'data': The data to update on the post.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.

#### client.deletePost( id, callback )

Deletes a post.

*NOTE:* Deleting a post may move it to the trash and then deleting a second time will actually delete.

* 'id': The ID of the post to delete.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.deleteTerm"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>deleteTerm ( taxonomy, id, fn )](#apidoc.element.wordpress.Client.prototype.deleteTerm)
- description and source-code
```javascript
deleteTerm = function ( taxonomy, id, fn ) {
		this.authenticatedCall( "wp.deleteTerm", taxonomy, id, fn );
	}
```
- example usage
```shell
...

Edits an existing taxonomy term.

* 'id': The ID of the taxonomy term to edit.
* 'data': The data to update on the taxonomy.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.

#### client.deleteTerm( taxonomy, id, callback )

Deletes a taxonomy term.

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'id': The ID of the taxonomy term to delete.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.editPost"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>editPost ( id, data, fn )](#apidoc.element.wordpress.Client.prototype.editPost)
- description and source-code
```javascript
editPost = function ( id, data, fn ) {
		this.authenticatedCall( "wp.editPost", id, fieldMap.to( data, "post" ), fn );
	}
```
- example usage
```shell
...

Creates a new post.

* 'data': The data for the new post.
* 'callback' ('function( error, id )'): A callback to invoke when the API call is complete.
  * 'id': The ID of the new post.

#### client.editPost( id, data, callback )

Edits an existing post.

* 'id': The ID of the post to edit.
* 'data': The data to update on the post.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.editTerm"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>editTerm ( id, data, fn )](#apidoc.element.wordpress.Client.prototype.editTerm)
- description and source-code
```javascript
editTerm = function ( id, data, fn ) {
		this.authenticatedCall( "wp.editTerm", id, fieldMap.to( data, "term" ), fn );
	}
```
- example usage
```shell
...

Creates a new taxonomy term.

* 'data': The data for the new taxonomy term.
* 'callback' ('function( error, id )'): A callback to invoke when the API call is complete.
  * 'id': The ID of the new taxonomy term.

#### client.editTerm( id, data, callback )

Edits an existing taxonomy term.

* 'id': The ID of the taxonomy term to edit.
* 'data': The data to update on the taxonomy.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getMediaItem"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getMediaItem ( id, fn )](#apidoc.element.wordpress.Client.prototype.getMediaItem)
- description and source-code
```javascript
getMediaItem = function ( id, fn ) {
		this.authenticatedCall( "wp.getMediaItem", id, function( error, media ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, fieldMap.from( media, "media" ) );
		});
	}
```
- example usage
```shell
...

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'id': The ID of the taxonomy term to delete.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.

### Media

#### client.getMediaItem( id, callback )

Gets a piece of media by ID.

* 'id': The ID of the piece of media to get.
* 'callback' ('function( error, media )' ): A callback to invoke when the API call is complete.

#### client.getMediaLibrary( [filter], callback )
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getMediaLibrary"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getMediaLibrary ( filter, fn )](#apidoc.element.wordpress.Client.prototype.getMediaLibrary)
- description and source-code
```javascript
getMediaLibrary = function ( filter, fn ) {
		if ( typeof filter === "function" ) {
			fn = filter;
			filter = {};
		}

		this.authenticatedCall( "wp.getMediaLibrary", filter, function( error, media ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, media.map(function( item ) {
				return fieldMap.from( item, "media" );
			}));
		});
	}
```
- example usage
```shell
...
#### client.getMediaItem( id, callback )

Gets a piece of media by ID.

* 'id': The ID of the piece of media to get.
* 'callback' ('function( error, media )' ): A callback to invoke when the API call is complete.

#### client.getMediaLibrary( [filter], callback )

* 'filter' (optional): A hash of key/value pairs for filtering which posts to get.
* 'callback' ('function( error, media )' ): A callback to invoke when the API call is complete.

#### client.uploadFile( data, callback )

Uploads a file to Wordpress.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getPost"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPost ( id, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPost)
- description and source-code
```javascript
getPost = function ( id, fields, fn ) {
		if ( typeof fields === "function" ) {
			fn = fields;
			fields = null;
		}

		if ( fields ) {
			fields = fieldMap.array( fields, "post" );
		}

		this.authenticatedCall( "wp.getPost", id, fields, function( error, post ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, fieldMap.from( post, "post" ) );
		});
	}
```
- example usage
```shell
...

#### wordpress.Client

The constructor used for client connections. Useful for creating extensions.

### Posts

#### client.getPost( id [, fields], callback )

Gets a post by ID.

* 'id': The ID of the post to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, post )'): A callback to invoke when the API call is complete.
* 'post': An object containing the post data.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getPostType"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPostType ( name, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPostType)
- description and source-code
```javascript
getPostType = function ( name, fields, fn ) {
		if ( typeof fields === "function" ) {
			fn = fields;
			fields = null;
		}

		if ( fields ) {
			fields = fieldMap.array( fields, "postType" );
		}

		this.authenticatedCall( "wp.getPostType", name, fields, function( error, postType ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, fieldMap.from( postType, "postType" ) );
		});
	}
```
- example usage
```shell
...
Deletes a post.

*NOTE:* Deleting a post may move it to the trash and then deleting a second time will actually delete.

* 'id': The ID of the post to delete.
* 'callback' ('function( error )'): A callback to invoke when the API call is complete.

#### client.getPostType( name, [, fields], callback )

Gets a post type by name.

* 'name': The name of the post type to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, postType )'): A callback to invoke when the API call is complete.
* 'postType': An object containing the post type data.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getPostTypes"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPostTypes ( filter, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPostTypes)
- description and source-code
```javascript
getPostTypes = function ( filter, fields, fn ) {
		if ( typeof filter === "function" ) {
			fn = filter;
			fields = null;
			filter = {};
		}

		if ( typeof fields === "function" ) {
			fn = fields;
			fields = null;
		}

		if ( Array.isArray(filter) ) {
			fields = filter;
			filter = {};
		}

		if ( fields ) {
			fields = fieldMap.array( fields, "postType" );
		}

		this.authenticatedCall( "wp.getPostTypes", filter, fields, function( error, postTypes ) {
			if ( error ) {
				return fn( error );
			}

			Object.keys( postTypes ).forEach(function( postType ) {
				postTypes[ postType ] = fieldMap.from( postTypes[ postType ], "postType" );
			});
			fn( null, postTypes );
		});
	}
```
- example usage
```shell
...
Gets a post type by name.

* 'name': The name of the post type to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, postType )'): A callback to invoke when the API call is complete.
* 'postType': An object containing the post type data.

#### client.getPostTypes( [filter], [, fields], callback )

Gets all post types.

* 'filter' (optional): A hash of key/value pairs for filtering which posts types to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, postTypes )'): A callback to invoke when the API call is complete.
* 'postTypes': An array containing the post types.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getPosts"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getPosts ( filter, fields, fn )](#apidoc.element.wordpress.Client.prototype.getPosts)
- description and source-code
```javascript
getPosts = function ( filter, fields, fn ) {
		if ( typeof filter === "function" ) {
			fn = filter;
			fields = null;
			filter = {};
		}

		if ( typeof fields === "function" ) {
			fn = fields;
			fields = null;
		}

		if ( filter.type ) {
			filter.post_type = filter.type;
			delete filter.type;
		}

		if ( filter.status ) {
			filter.post_status = filter.status;
			delete filter.status;
		}

		if ( filter.orderby ) {
			filter.orderby = fieldMap.array( [ filter.orderby ], "post" )[ 0 ];
		}

		if ( fields ) {
			fields = fieldMap.array( fields, "post" );
		}

		this.authenticatedCall( "wp.getPosts", filter, fields, function( error, posts ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, posts.map(function( post ) {
				return fieldMap.from( post, "post" );
			}));
		});
	}
```
- example usage
```shell
...
var wordpress = require( "wordpress" );
var client = wordpress.createClient({
	url: "my-site.com",
	username: "admin",
	password: "secret"
});

client.getPosts(function( error, posts ) {
	console.log( "Found " + posts.length + " posts!" );
});
'''

More usage examples can be found in the 'examples' directory.

### Full Site Synchronization
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getTaxonomies"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTaxonomies ( fn )](#apidoc.element.wordpress.Client.prototype.getTaxonomies)
- description and source-code
```javascript
getTaxonomies = function ( fn ) {
		this.authenticatedCall( "wp.getTaxonomies", function( error, taxonomies ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, taxonomies.map(function( taxonomy ) {
				return fieldMap.from( taxonomy, "taxonomy" );
			}));
		});
	}
```
- example usage
```shell
...

Gets a taxonomy by name.

* 'name': The name of the taxonomy to get.
* 'callback' ('function( error, taxonomy )'): A callback to invoke when the API call is complete.
  * 'taxonomy': An object containing the taxonomy data.

#### client.getTaxonomies( callback )

Gets all taxonomies.

* 'callback' ('function( error, taxonomies )'): A callback to invoke when the API call is complete.
  * 'taxonomies': An array containing the taxonomies.

#### client.getTerm( taxonomy, id, callback )
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getTaxonomy"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTaxonomy ( name, fn )](#apidoc.element.wordpress.Client.prototype.getTaxonomy)
- description and source-code
```javascript
getTaxonomy = function ( name, fn ) {
		this.authenticatedCall( "wp.getTaxonomy", name, function( error, taxonomy ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, fieldMap.from( taxonomy, "taxonomy" ) );
		});
	}
```
- example usage
```shell
...
* 'filter' (optional): A hash of key/value pairs for filtering which posts types to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, postTypes )'): A callback to invoke when the API call is complete.
* 'postTypes': An array containing the post types.

### Taxonomies

#### client.getTaxonomy( name, callback )

Gets a taxonomy by name.

* 'name': The name of the taxonomy to get.
* 'callback' ('function( error, taxonomy )'): A callback to invoke when the API call is complete.
* 'taxonomy': An object containing the taxonomy data.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getTerm"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTerm ( taxonomy, id, fn )](#apidoc.element.wordpress.Client.prototype.getTerm)
- description and source-code
```javascript
getTerm = function ( taxonomy, id, fn ) {
		this.authenticatedCall( "wp.getTerm", taxonomy, id, function( error, term ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, fieldMap.from( term, "term" ) );
		});
	}
```
- example usage
```shell
...
#### client.getTaxonomies( callback )

Gets all taxonomies.

* 'callback' ('function( error, taxonomies )'): A callback to invoke when the API call is complete.
* 'taxonomies': An array containing the taxonomies.

#### client.getTerm( taxonomy, id, callback )

Gets a taxonomy term by ID.

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'id': The ID of the term to get.
* 'callback' ('function( error, term )'): A callback to invoke when the API call is complete.
* 'term': An object containing the taxonomy term data.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.getTerms"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>getTerms ( taxonomy, filter, fn )](#apidoc.element.wordpress.Client.prototype.getTerms)
- description and source-code
```javascript
getTerms = function ( taxonomy, filter, fn ) {
		if ( typeof filter === "function" ) {
			fn = filter;
			filter = {};
		}

		if ( filter.hideEmpty ) {
			filter.hide_empty = filter.hideEmpty;
			delete filter.hideEmpty;
		}

		if ( filter.orderby ) {
			filter.orderby = fieldMap.array( [ filter.orderby ], "term" )[ 0 ];
		}

		this.authenticatedCall( "wp.getTerms", taxonomy, filter, function( error, terms ) {
			if ( error ) {
				return fn( error );
			}

			fn( null, terms.map(function( term ) {
				return fieldMap.from( term, "term" );
			}));
		});
	}
```
- example usage
```shell
...
Gets a taxonomy term by ID.

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'id': The ID of the term to get.
* 'callback' ('function( error, term )'): A callback to invoke when the API call is complete.
* 'term': An object containing the taxonomy term data.

#### client.getTerms( taxonomy [, fields], callback )

Gets all taxonomy terms.

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, terms )'): A callback to invoke when the API call is complete.
* 'terms': An array containing the taxonomy terms.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.listMethods"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>listMethods ( fn )](#apidoc.element.wordpress.Client.prototype.listMethods)
- description and source-code
```javascript
listMethods = function ( fn ) {
		this.call( "system.listMethods", fn );
	}
```
- example usage
```shell
...
  * 'overwrite' (optional): Whether this file should overwrite any existing file of the same name.
  * 'postId' (optional): Which post to assign the attachment to.
* 'callback' ('function( error, file )'): A callback to invoke when the API call is complete.
  * 'file': An object containing the file data.

### Utilities

#### client.listMethods( callback )

Gets a list of all avaialble methods.

* 'callback' ('function( error, methods )'): A callback to invoke when the API call is complete.
  * 'methods': An array of methods.

#### client.call( method [, args... ], callback )
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.newPost"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>newPost ( data, fn )](#apidoc.element.wordpress.Client.prototype.newPost)
- description and source-code
```javascript
newPost = function ( data, fn ) {
		this.authenticatedCall( "wp.newPost", fieldMap.to( data, "post" ), fn );
	}
```
- example usage
```shell
...
Gets all posts, optionally filtered.

* 'filter' (optional): A hash of key/value pairs for filtering which posts to get.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, posts )'): A callback to invoke when the API call is complete.
* 'posts': An array containing the posts.

#### client.newPost( data, callback )

Creates a new post.

* 'data': The data for the new post.
* 'callback' ('function( error, id )'): A callback to invoke when the API call is complete.
* 'id': The ID of the new post.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.newTerm"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>newTerm ( data, fn )](#apidoc.element.wordpress.Client.prototype.newTerm)
- description and source-code
```javascript
newTerm = function ( data, fn ) {
		this.authenticatedCall( "wp.newTerm", fieldMap.to( data, "term" ), fn );
	}
```
- example usage
```shell
...
Gets all taxonomy terms.

* 'taxonomy': The name fo the taxonomy the term belongs to.
* 'fields' (optional): An array of fields to return.
* 'callback' ('function( error, terms )'): A callback to invoke when the API call is complete.
* 'terms': An array containing the taxonomy terms.

#### client.newTerm( data, callback )

Creates a new taxonomy term.

* 'data': The data for the new taxonomy term.
* 'callback' ('function( error, id )'): A callback to invoke when the API call is complete.
* 'id': The ID of the new taxonomy term.
...
```

#### <a name="apidoc.element.wordpress.Client.prototype.uploadFile"></a>[function <span class="apidocSignatureSpan">wordpress.Client.prototype.</span>uploadFile ( data, fn )](#apidoc.element.wordpress.Client.prototype.uploadFile)
- description and source-code
```javascript
uploadFile = function ( data, fn ) {
		this.authenticatedCall( "wp.uploadFile", fieldMap.to( data, "file" ), fn );
	}
```
- example usage
```shell
...
* 'callback' ('function( error, media )' ): A callback to invoke when the API call is complete.

#### client.getMediaLibrary( [filter], callback )

* 'filter' (optional): A hash of key/value pairs for filtering which posts to get.
* 'callback' ('function( error, media )' ): A callback to invoke when the API call is complete.

#### client.uploadFile( data, callback )

Uploads a file to Wordpress.

* 'data': The data for the file to upload.
* 'name': The filename.
* 'type': The file MIME type, e.g 'img/jpg'.
* 'bits': Binary data.
...
```



# <a name="apidoc.module.wordpress.fieldMap"></a>[module wordpress.fieldMap](#apidoc.module.wordpress.fieldMap)

#### <a name="apidoc.element.wordpress.fieldMap.array"></a>[function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>array ( data, type )](#apidoc.element.wordpress.fieldMap.array)
- description and source-code
```javascript
array = function ( data, type ) {
		var map = maps[ type ].renames;
		return data.map(function( field ) {
			return map[ field ];
		});
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wordpress.fieldMap.from"></a>[function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>from ( data, type )](#apidoc.element.wordpress.fieldMap.from)
- description and source-code
```javascript
from = function ( data, type ) {
		return mapFields( data, maps[ type ].from );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.wordpress.fieldMap.to"></a>[function <span class="apidocSignatureSpan">wordpress.fieldMap.</span>to ( data, type )](#apidoc.element.wordpress.fieldMap.to)
- description and source-code
```javascript
to = function ( data, type ) {
		return mapFields( data, maps[ type ].to );
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
