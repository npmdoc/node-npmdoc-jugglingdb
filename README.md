# api documentation for  [jugglingdb (v1.0.2)](https://github.com/1602/jugglingdb)  [![npm package](https://img.shields.io/npm/v/npmdoc-jugglingdb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jugglingdb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jugglingdb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jugglingdb)
#### ORM for every database: redis, mysql, neo4j, mongodb, couchdb, postgres, sqlite

[![NPM](https://nodei.co/npm/jugglingdb.png?downloads=true)](https://www.npmjs.com/package/jugglingdb)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jugglingdb/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jugglingdb_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jugglingdb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jugglingdb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jugglingdb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Anatoliy Chakkaev",
        "email": "rpm1602@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/1602/jugglingdb/issues"
    },
    "contributors": [
        {
            "name": "Anatoliy Chakkaev",
            "email": "rpm1602@gmail.com"
        },
        {
            "name": "Julien Guimont",
            "email": "julien.guimont@gmail.com"
        },
        {
            "name": "Joseph Junker",
            "email": "joseph.jnk@gmail.com"
        },
        {
            "name": "Henri Bergius",
            "email": "henri.bergius@iki.fi"
        },
        {
            "name": "redvulps",
            "email": "fabopereira@gmail.com"
        },
        {
            "name": "Felipe Sateler",
            "email": "fsateler@gmail.com"
        },
        {
            "name": "Amir M. Mahmoudi",
            "email": "a@geeknux.com"
        },
        {
            "name": "Justinas Stankevičius",
            "email": "justinas@justinas.me"
        },
        {
            "name": "Rick O'Toole",
            "email": "patrick.n.otoole@gmail.com"
        },
        {
            "name": "Nicholas Westlake",
            "email": "nicholasredlin@gmail.com"
        }
    ],
    "dependencies": {
        "inflection": "=1.2.7",
        "should": "=6.0.3",
        "when": "3.7.3"
    },
    "description": "ORM for every database: redis, mysql, neo4j, mongodb, couchdb, postgres, sqlite",
    "devDependencies": {
        "jshint": "2.5.6",
        "mocha": "~1.8.2",
        "semicov": "*",
        "should": "~3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "c3ff07dc89d01d4b940fd1ed2282d29e0ca26b15",
        "tarball": "https://registry.npmjs.org/jugglingdb/-/jugglingdb-1.0.2.tgz"
    },
    "engines": [
        "node >= 0.6"
    ],
    "homepage": "https://github.com/1602/jugglingdb",
    "jshintConfig": {
        "proto": true
    },
    "main": "index.js",
    "maintainers": [
        {
            "name": "anatoliy",
            "email": "rpm1602@gmail.com"
        }
    ],
    "man": [
        "./docs/man/jugglingdb.3",
        "./docs/man/schema.3",
        "./docs/man/model.3",
        "./docs/man/hooks.3",
        "./docs/man/validations.3",
        "./docs/man/roadmap.3",
        "./docs/man/changelog.3"
    ],
    "name": "jugglingdb",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/1602/jugglingdb.git"
    },
    "scripts": {
        "prepublish": "make build",
        "test": "make test"
    },
    "version": "1.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jugglingdb](#apidoc.module.jugglingdb)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>AbstractClass {{signature}}](#apidoc.element.jugglingdb.AbstractClass)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>BaseSQL ()](#apidoc.element.jugglingdb.BaseSQL)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>Schema (name, settings)](#apidoc.element.jugglingdb.Schema)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>init (compound)](#apidoc.element.jugglingdb.init)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>list (data, type, parent)](#apidoc.element.jugglingdb.list)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>loadSchema (filename, settings, compound)](#apidoc.element.jugglingdb.loadSchema)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>test (exportCasesHere, schema)](#apidoc.element.jugglingdb.test)
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>AbstractClass.prototype
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>BaseSQL.prototype
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>Schema.prototype
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>Schema.types
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>jutil
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>list.prototype
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>schema
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>scope
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>utils
1.  object <span class="apidocSignatureSpan">jugglingdb.</span>validations
1.  string <span class="apidocSignatureSpan">jugglingdb.</span>version

#### [module jugglingdb.AbstractClass](#apidoc.module.jugglingdb.AbstractClass)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>AbstractClass {{signature}}](#apidoc.element.jugglingdb.AbstractClass.AbstractClass)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>_forDB (data)](#apidoc.element.jugglingdb.AbstractClass._forDB)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>_fromDB (data)](#apidoc.element.jugglingdb.AbstractClass._fromDB)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>all ()](#apidoc.element.jugglingdb.AbstractClass.all)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>belongsTo (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.belongsTo)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>count ()](#apidoc.element.jugglingdb.AbstractClass.count)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>create ()](#apidoc.element.jugglingdb.AbstractClass.create)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>defineProperty (prop, params)](#apidoc.element.jugglingdb.AbstractClass.defineProperty)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>destroyAll ()](#apidoc.element.jugglingdb.AbstractClass.destroyAll)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>exists ()](#apidoc.element.jugglingdb.AbstractClass.exists)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>find ()](#apidoc.element.jugglingdb.AbstractClass.find)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>findOne ()](#apidoc.element.jugglingdb.AbstractClass.findOne)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>findOrCreate (query, data, callback)](#apidoc.element.jugglingdb.AbstractClass.findOrCreate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>hasAndBelongsToMany (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.hasAndBelongsToMany)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>hasMany (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.hasMany)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>include (objects, include, cb)](#apidoc.element.jugglingdb.AbstractClass.include)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>iterate (filter, iterator, callback)](#apidoc.element.jugglingdb.AbstractClass.iterate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>relationNameFor (foreignKey)](#apidoc.element.jugglingdb.AbstractClass.relationNameFor)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>scope (name, params)](#apidoc.element.jugglingdb.AbstractClass.scope)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>toString ()](#apidoc.element.jugglingdb.AbstractClass.toString)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>update ()](#apidoc.element.jugglingdb.AbstractClass.update)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>updateOrCreate ()](#apidoc.element.jugglingdb.AbstractClass.updateOrCreate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>upsert ()](#apidoc.element.jugglingdb.AbstractClass.upsert)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validate ()](#apidoc.element.jugglingdb.AbstractClass.validate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validateAsync ()](#apidoc.element.jugglingdb.AbstractClass.validateAsync)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesExclusionOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesExclusionOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesFormatOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesFormatOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesInclusionOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesInclusionOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesLengthOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesLengthOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesNumericalityOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesNumericalityOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesPresenceOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesPresenceOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesUniquenessOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesUniquenessOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>whatTypeName (propName)](#apidoc.element.jugglingdb.AbstractClass.whatTypeName)
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterCreate
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterDestroy
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterInitialize
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterSave
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterUpdate
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>afterValidate
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>beforeCreate
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>beforeDestroy
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>beforeSave
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>beforeUpdate
1.  object <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>beforeValidate

#### [module jugglingdb.AbstractClass.prototype](#apidoc.module.jugglingdb.AbstractClass.prototype)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>_adapter ()](#apidoc.element.jugglingdb.AbstractClass.prototype._adapter)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>_initProperties (data, applySetters)](#apidoc.element.jugglingdb.AbstractClass.prototype._initProperties)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>destroy ()](#apidoc.element.jugglingdb.AbstractClass.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>fromObject (obj)](#apidoc.element.jugglingdb.AbstractClass.prototype.fromObject)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>inspect ()](#apidoc.element.jugglingdb.AbstractClass.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>isNewRecord ()](#apidoc.element.jugglingdb.AbstractClass.prototype.isNewRecord)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>isValid (callback, data)](#apidoc.element.jugglingdb.AbstractClass.prototype.isValid)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>propertyChanged (attr)](#apidoc.element.jugglingdb.AbstractClass.prototype.propertyChanged)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>reload ()](#apidoc.element.jugglingdb.AbstractClass.prototype.reload)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>reset ()](#apidoc.element.jugglingdb.AbstractClass.prototype.reset)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>save ()](#apidoc.element.jugglingdb.AbstractClass.prototype.save)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>toJSON ()](#apidoc.element.jugglingdb.AbstractClass.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>toObject (onlySchema, cachedRelations)](#apidoc.element.jugglingdb.AbstractClass.prototype.toObject)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>trigger (actionName, work, data, quit)](#apidoc.element.jugglingdb.AbstractClass.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>updateAttribute ()](#apidoc.element.jugglingdb.AbstractClass.prototype.updateAttribute)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>updateAttributes ()](#apidoc.element.jugglingdb.AbstractClass.prototype.updateAttributes)
1.  [function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>whatTypeName (propName)](#apidoc.element.jugglingdb.AbstractClass.prototype.whatTypeName)

#### [module jugglingdb.BaseSQL](#apidoc.module.jugglingdb.BaseSQL)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>BaseSQL ()](#apidoc.element.jugglingdb.BaseSQL.BaseSQL)

#### [module jugglingdb.BaseSQL.prototype](#apidoc.module.jugglingdb.BaseSQL.prototype)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>automigrate (cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.automigrate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>command (sql, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.command)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>count (model, callback, where)](#apidoc.element.jugglingdb.BaseSQL.prototype.count)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>createTable (model, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.createTable)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>define (descr)](#apidoc.element.jugglingdb.BaseSQL.prototype.define)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>defineProperty (model, prop, params)](#apidoc.element.jugglingdb.BaseSQL.prototype.defineProperty)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>destroy (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>destroyAll (model, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.destroyAll)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>disconnect ()](#apidoc.element.jugglingdb.BaseSQL.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>dropTable (model, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.dropTable)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>escapeId (id)](#apidoc.element.jugglingdb.BaseSQL.prototype.escapeId)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>escapeName (name)](#apidoc.element.jugglingdb.BaseSQL.prototype.escapeName)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>exists (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.exists)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>find (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.find)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>query ()](#apidoc.element.jugglingdb.BaseSQL.prototype.query)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>queryOne (sql, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.queryOne)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>save (model, data, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.save)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>table (model)](#apidoc.element.jugglingdb.BaseSQL.prototype.table)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>tableEscaped (model)](#apidoc.element.jugglingdb.BaseSQL.prototype.tableEscaped)
1.  [function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>updateAttributes (model, id, data, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.updateAttributes)

#### [module jugglingdb.Schema](#apidoc.module.jugglingdb.Schema)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>Schema (name, settings)](#apidoc.element.jugglingdb.Schema.Schema)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>JSON ()](#apidoc.element.jugglingdb.Schema.JSON)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>Text (s)](#apidoc.element.jugglingdb.Schema.Text)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>registerType (type)](#apidoc.element.jugglingdb.Schema.registerType)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>super_ ()](#apidoc.element.jugglingdb.Schema.super_)
1.  object <span class="apidocSignatureSpan">jugglingdb.Schema.</span>types

#### [module jugglingdb.Schema.prototype](#apidoc.module.jugglingdb.Schema.prototype)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>automigrate (cb)](#apidoc.element.jugglingdb.Schema.prototype.automigrate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>autoupdate (cb)](#apidoc.element.jugglingdb.Schema.prototype.autoupdate)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>copyModel (Master)](#apidoc.element.jugglingdb.Schema.prototype.copyModel)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>define (className, properties, settings)](#apidoc.element.jugglingdb.Schema.prototype.define)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>defineForeignKey (className, key, foreignClassName)](#apidoc.element.jugglingdb.Schema.prototype.defineForeignKey)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>defineProperty (model, prop, params)](#apidoc.element.jugglingdb.Schema.prototype.defineProperty)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>disconnect (cb)](#apidoc.element.jugglingdb.Schema.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>extendModel (model, props)](#apidoc.element.jugglingdb.Schema.prototype.extendModel)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>freeze ()](#apidoc.element.jugglingdb.Schema.prototype.freeze)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>isActual (cb)](#apidoc.element.jugglingdb.Schema.prototype.isActual)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>log (sql, t)](#apidoc.element.jugglingdb.Schema.prototype.log)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>tableName (modelName)](#apidoc.element.jugglingdb.Schema.prototype.tableName)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>transaction ()](#apidoc.element.jugglingdb.Schema.prototype.transaction)

#### [module jugglingdb.Schema.types](#apidoc.module.jugglingdb.Schema.types)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.types.</span>JSON ()](#apidoc.element.jugglingdb.Schema.types.JSON)
1.  [function <span class="apidocSignatureSpan">jugglingdb.Schema.types.</span>Text (s)](#apidoc.element.jugglingdb.Schema.types.Text)

#### [module jugglingdb.jutil](#apidoc.module.jugglingdb.jutil)
1.  [function <span class="apidocSignatureSpan">jugglingdb.jutil.</span>inherits (newClass, baseClass)](#apidoc.element.jugglingdb.jutil.inherits)

#### [module jugglingdb.list](#apidoc.module.jugglingdb.list)
1.  [function <span class="apidocSignatureSpan">jugglingdb.</span>list (data, type, parent)](#apidoc.element.jugglingdb.list.list)

#### [module jugglingdb.list.prototype](#apidoc.module.jugglingdb.list.prototype)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>autoincrement ()](#apidoc.element.jugglingdb.list.prototype.autoincrement)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>concat ()](#apidoc.element.jugglingdb.list.prototype.concat)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>every ()](#apidoc.element.jugglingdb.list.prototype.every)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>filter ()](#apidoc.element.jugglingdb.list.prototype.filter)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>find (pattern, field)](#apidoc.element.jugglingdb.list.prototype.find)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>forEach ()](#apidoc.element.jugglingdb.list.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>indexOf ()](#apidoc.element.jugglingdb.list.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>inspect ()](#apidoc.element.jugglingdb.list.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>join ()](#apidoc.element.jugglingdb.list.prototype.join)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>lastIndexOf ()](#apidoc.element.jugglingdb.list.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>map (cb)](#apidoc.element.jugglingdb.list.prototype.map)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>pop ()](#apidoc.element.jugglingdb.list.prototype.pop)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>push (obj)](#apidoc.element.jugglingdb.list.prototype.push)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>remove (obj)](#apidoc.element.jugglingdb.list.prototype.remove)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>removeAt (index)](#apidoc.element.jugglingdb.list.prototype.removeAt)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>reverse ()](#apidoc.element.jugglingdb.list.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>shift ()](#apidoc.element.jugglingdb.list.prototype.shift)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>slice ()](#apidoc.element.jugglingdb.list.prototype.slice)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>some ()](#apidoc.element.jugglingdb.list.prototype.some)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>sort ()](#apidoc.element.jugglingdb.list.prototype.sort)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>splice ()](#apidoc.element.jugglingdb.list.prototype.splice)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toJSON ()](#apidoc.element.jugglingdb.list.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toObject ()](#apidoc.element.jugglingdb.list.prototype.toObject)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toSource ()](#apidoc.element.jugglingdb.list.prototype.toSource)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toString ()](#apidoc.element.jugglingdb.list.prototype.toString)
1.  [function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>unshift ()](#apidoc.element.jugglingdb.list.prototype.unshift)

#### [module jugglingdb.schema](#apidoc.module.jugglingdb.schema)
1.  [function <span class="apidocSignatureSpan">jugglingdb.schema.</span>Schema (name, settings)](#apidoc.element.jugglingdb.schema.Schema)

#### [module jugglingdb.scope](#apidoc.module.jugglingdb.scope)
1.  [function <span class="apidocSignatureSpan">jugglingdb.scope.</span>defineScope (cls, targetClass, name, params, methods)](#apidoc.element.jugglingdb.scope.defineScope)

#### [module jugglingdb.utils](#apidoc.module.jugglingdb.utils)
1.  [function <span class="apidocSignatureSpan">jugglingdb.utils.</span>safeRequire (module)](#apidoc.element.jugglingdb.utils.safeRequire)

#### [module jugglingdb.validations](#apidoc.module.jugglingdb.validations)
1.  [function <span class="apidocSignatureSpan">jugglingdb.validations.</span>ValidationError (obj)](#apidoc.element.jugglingdb.validations.ValidationError)



# <a name="apidoc.module.jugglingdb"></a>[module jugglingdb](#apidoc.module.jugglingdb)

#### <a name="apidoc.element.jugglingdb.AbstractClass"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>AbstractClass {{signature}}](#apidoc.element.jugglingdb.AbstractClass)
- description and source-code
```javascript
[Model undefined]
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>BaseSQL ()](#apidoc.element.jugglingdb.BaseSQL)
- description and source-code
```javascript
function BaseSQL() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>Schema (name, settings)](#apidoc.element.jugglingdb.Schema)
- description and source-code
```javascript
function Schema(name, settings) {
    var schema = this;
    // just save everything we get
    this.name = name;
    this.settings = settings || {};

    // Disconnected by default
    this.connected = false;
    this.connecting = false;

    // create blank models pool
    this.models = {};
    this.definitions = {};

    if (this.settings.log) {
        this.on('log', function(str, duration) {
            console.log(str);
        });
    }

    // and initialize schema using adapter
    // this is only one initialization entry point of adapter
    // this module should define 'adapter' member of 'this' (schema)
    var adapter;
    if (typeof name === 'object') {
        adapter = name;
        this.name = adapter.name;
    } else if (name.match(/^\//)) {
        // try absolute path
        adapter = require(name);
    } else if (existsSync(__dirname + '/adapters/' + name + '.js')) {
        // try built-in adapter
        adapter = require('./adapters/' + name);
    } else {
        // try foreign adapter
        try {
            adapter = require('jugglingdb-' + name);
        } catch (e) {
            return console.log('\nWARNING: JugglingDB adapter "' + name + '" is not installed,\nso your models would not work, to
 fix run:\n\n    npm install jugglingdb-' + name, '\n');
        }
    }

    this.connecting = true;
    adapter.initialize(this, function () {

        this.adapter.log = function (query, start) {
            schema.log(query, start);
        };

        this.adapter.logger = function (query) {
            var t1 = Date.now();
            var log = this.log;
            return function (q) {
                log(q || query, t1);
            };
        };

        this.connecting = false;
        this.connected = true;
        this.emit('connected');

    }.bind(this));

    // we have an adaper now?
    if (!this.adapter) {
        this.emit('disconnected');
        throw new Error('Adapter "' + name + '" is not defined correctly: it should define 'adapter' member of schema synchronously
');
    }

    schema.connect = function(cb) {
        var schema = this;
        schema.connecting = true;
        return new when.Promise(function(resolve, reject) {
            if (!schema.adapter.connect) {
                return process.nextTick(function() {
                    schema.connecting = false;
                    if (cb) {
                        cb(null, schema);
                    }
                    return resolve(schema);
                });
            }
            schema.adapter.connect(function(err) {
                if (err) {
                    schema.connected = false;
                    schema.connecting = false;
                    reject(err);
                    if (cb) {
                        cb(err);
                    }
                } else {
                    schema.connected = true;
                    schema.connecting = false;
                    schema.emit('connected');
                    resolve(schema);
                    if (cb) {
                        cb(null, schema);
                    }
                }
            });
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.init"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>init (compound)](#apidoc.element.jugglingdb.init)
- description and source-code
```javascript
init = function (compound) {
    if (global.railway) {
        global.railway.orm = exports;
    } else {
        compound.orm = {
            Schema: exports.Schema,
            AbstractClass: exports.AbstractClass
        };
        if (compound.app.enabled('noeval schema')) {
            compound.orm.schema = exports.loadSchema(
                compound.root + '/db/schema',
                compound.app.get('database'),
                compound
            );
            if (compound.app.enabled('autoupdate')) {
                compound.on('ready', function() {
                    compound.orm.schema.forEach(function(s) {
                        s.autoupdate();
                        if (s.backyard) {
                            s.backyard.autoupdate();
                            s.backyard.log = s.log;
                        }
                    });
                });
            }
            return;
        }
    }

    // legacy stuff

    if (compound.version > '1.1.5-15') {
        compound.on('after routes', initialize);
    } else {
        initialize();
    }

    function initialize() {
        var railway = './lib/railway', init;
        try {
            init = require(railway);
        } catch (e) {
            console.log(e.stack);
        }
        if (init) {
            init(compound);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>list (data, type, parent)](#apidoc.element.jugglingdb.list)
- description and source-code
```javascript
function List(data, type, parent) {
    var list = this;
    if (!(list instanceof List)) {
        return new List(data);
    }

    if (data && data instanceof List) data = data.items;

    Object.defineProperty(list, 'parent', {
        writable: false,
        enumerable: false,
        configurable: false,
        value: parent
    });

    Object.defineProperty(list, 'nextid', {
        writable: true,
        enumerable: false,
        value: 1
    });

    var Item = ListItem;
    if (typeof type === 'object' && type.constructor.name === 'Array') {
        Item = type[0] || ListItem;
    }

    data = list.items = data || [];
    Object.defineProperty(list, 'ItemType', {
        writable: true,
        enumerable: false,
        configurable: true,
        value: Item
    });

    if ('string' === typeof data) {
        try {
            list.items = data = JSON.parse(data);
        } catch(e) {
            list.items = data = [];
        }
    }

    data.forEach(function(item, i) {
        data[i] = new Item(item, list);
        Object.defineProperty(list, data[i].id, {
            writable: true,
            enumerable: false,
            configurable: true,
            value: data[i]
        });
        if (list.nextid <= data[i].id) {
            list.nextid = data[i].id + 1;
        }
    });

    Object.defineProperty(list, 'length', {
        enumerable: false,
        configurable: true,
        get: function() {
            return list.items.length;
        }
    });

    return list;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.loadSchema"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>loadSchema (filename, settings, compound)](#apidoc.element.jugglingdb.loadSchema)
- description and source-code
```javascript
loadSchema = function (filename, settings, compound) {
    var schema = [];
    var definitions = require(filename);
    Object.keys(definitions).forEach(function(k) {
        var conf = settings[k];
        if (!conf) {
            console.log('No config found for ' + k + ' schema, using in-memory schema');
            conf = {driver: 'memory'};
        }
        schema[k] = new Schema(conf.driver, conf);
        schema[k].on('define', function(m, name, prop, sett) {
            compound.models[name] = m;
            if (conf.backyard) {
                schema[k].backyard.define(name, prop, sett);
            }
        });
        schema[k].name = k;
        schema.push(schema[k]);
        if (conf.backyard) {
            schema[k].backyard = new Schema(conf.backyard.driver, conf.backyard);
        }
        if ('function' === typeof definitions[k]) {
            define(schema[k], definitions[k]);
            if (conf.backyard) {
                define(schema[k].backyard, definitions[k]);
            }
        }
    });

    return schema;

    function define(db, def) {
        def(db, compound);
    }
}
```
- example usage
```shell
...
    global.railway.orm = exports;
} else {
    compound.orm = {
        Schema: exports.Schema,
        AbstractClass: exports.AbstractClass
    };
    if (compound.app.enabled('noeval schema')) {
        compound.orm.schema = exports.loadSchema(
            compound.root + '/db/schema',
            compound.app.get('database'),
            compound
        );
        if (compound.app.enabled('autoupdate')) {
            compound.on('ready', function() {
                compound.orm.schema.forEach(function(s) {
...
```

#### <a name="apidoc.element.jugglingdb.test"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>test (exportCasesHere, schema)](#apidoc.element.jugglingdb.test)
- description and source-code
```javascript
function testSchema(exportCasesHere, schema) {

    batch = exportCasesHere;
    schemaName = schema.name;
    if (schema.name.match(/^\/.*\/test\/\.\.$/)) {
        schemaName = schemaName.split('/').slice(-3).shift();
    }
    var start;

    batch['should connect to database'] = function (test) {
        start = Date.now();
        if (schema.connected) return test.done();
        schema.on('connected', test.done);
    };

    schema.log = function (a) {
        console.log(a);
        nbSchemaRequests++;
    };

    batch[schemaName] = {};

    testOrm(schema);

    batch['all tests done'] = function (test) {
        test.done();
        process.nextTick(allTestsDone);
    };

    function allTestsDone() {
        schema.disconnect();
        console.log('Test done in %dms\n', Date.now() - start);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.AbstractClass"></a>[module jugglingdb.AbstractClass](#apidoc.module.jugglingdb.AbstractClass)

#### <a name="apidoc.element.jugglingdb.AbstractClass.AbstractClass"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>AbstractClass {{signature}}](#apidoc.element.jugglingdb.AbstractClass.AbstractClass)
- description and source-code
```javascript
[Model undefined]
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass._forDB"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>_forDB (data)](#apidoc.element.jugglingdb.AbstractClass._forDB)
- description and source-code
```javascript
_forDB = function (data) {
    if (!data) return;
    var res = {};
    var definition = this.schema.definitions[this.modelName].properties;
    Object.keys(data).forEach(function (propName) {
        var val;
        var typeName = this.whatTypeName(propName);
        if (!typeName && !data[propName] instanceof Array) {
            return;
        }
        val = data[propName];
        if (definition[propName] && definition[propName].name) {
          // Use different name for DB field/column
          res[definition[propName].name] = val;
        } else {
          res[propName] = val;
        }
    }.bind(this));
    return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass._fromDB"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>_fromDB (data)](#apidoc.element.jugglingdb.AbstractClass._fromDB)
- description and source-code
```javascript
_fromDB = function (data) {
    if (!data) return;
    var definition = this.schema.definitions[this.modelName].properties;
    var propNames = Object.keys(data);
    Object.keys(definition).forEach(function (defPropName) {
      var customName = definition[defPropName].name;
      if (customName && propNames.indexOf(customName) !== -1) {
        data[defPropName] = data[customName];
        delete data[customName];
      }
    });
    return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.all"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>all ()](#apidoc.element.jugglingdb.AbstractClass.all)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// Common API methods

// just instantiate model
new Post
// save model (of course async)
Post.create(cb);
// all posts
Post.all(cb)
// all posts by user
Post.all({where: {userId: user.id}, order: 'id', limit: 10, skip: 20}, cb);
// the same as prev
user.posts(cb)
// get one latest post
Post.findOne({where: {published: true}, order: 'date DESC'}, cb);
// same as new Post({userId: user.id});
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.belongsTo"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>belongsTo (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.belongsTo)
- description and source-code
```javascript
belongsTo = function (anotherClass, params) {
    params = params || {};
    if ('string' === typeof anotherClass) {
        params.as = anotherClass;
        if (params.model) {
            anotherClass = params.model;
        } else {
            var anotherClassName = anotherClass.toLowerCase();
            for(var name in this.schema.models) {
                if (name.toLowerCase() === anotherClassName) {
                    anotherClass = this.schema.models[name];
                }
            }
        }
    }
    var methodName = params.as || i8n.camelize(anotherClass.modelName, true);
    var fk = params.foreignKey || methodName + 'Id';

    this.relations[methodName] = {
        type: 'belongsTo',
        keyFrom: fk,
        keyTo: 'id',
        modelTo: anotherClass,
        multiple: false
    };

    this.schema.defineForeignKey(this.modelName, fk, anotherClass.modelName);
    this.prototype.__finders__ = this.prototype.__finders__ || {};

    this.prototype.__finders__[methodName] = function (id, cb) {
        if (id === null) {
            cb(null, null);
            return;
        }
        anotherClass.find(id, function (err,inst) {
            if (err) {
                return cb(err);
            }
            if (!inst) {
                return cb(null, null);
            }
            if (inst.id.toString() === this[fk].toString()) {
                cb(null, inst);
            } else {
                cb(new Error('Permission denied'));
            }
        }.bind(this));
    };

    this.prototype[methodName] = function (refresh, p) {
        if (arguments.length === 1) {
            p = refresh;
            refresh = false;
        } else if (arguments.length > 2) {
            throw new Error('Method can\'t be called with more than two arguments');
        }
        var self = this;
        var cachedValue;
        if (!refresh && this.__cachedRelations && (typeof this.__cachedRelations[methodName] !== 'undefined')) {
            cachedValue = this.__cachedRelations[methodName];
        }
        if (p instanceof Model) { // acts as setter
            this[fk] = p.id;
            this.__cachedRelations[methodName] = p;
        } else if (typeof p === 'function') { // acts as async getter
            if (typeof cachedValue === 'undefined') {
                this.__finders__[methodName].apply(self, [this[fk], function(err, inst) {
                    if (!err) {
                        self.__cachedRelations[methodName] = inst;
                    }
                    p(err, inst);
                }]);
                return this[fk];
            } else {
                p(null, cachedValue);
                return cachedValue;
            }
        } else if (typeof p === 'undefined') { // acts as sync getter
            return this[fk];
        } else { // setter
            this[fk] = p;
            delete this.__cachedRelations[methodName];
        }
    };

}
```
- example usage
```shell
...
// setup relationships
User.hasMany(Post,   {as: 'posts',  foreignKey: 'userId'});
// creates instance methods:
// user.posts(conds)
// user.posts.build(data) // like new Post({userId: user.id});
// user.posts.create(data) // build and save

Post.belongsTo(User, {as: 'author', foreignKey: 'userId'});
// creates instance methods:
// post.author(callback) -- getter when called with function
// post.author() -- sync getter when called without params
// post.author(user) -- setter when called with object

User.hasAndBelongsToMany('groups');
// user.groups(callback) - get groups of user
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.count"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>count ()](#apidoc.element.jugglingdb.AbstractClass.count)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.create"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>create ()](#apidoc.element.jugglingdb.AbstractClass.create)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...

'''javascript
// setup relationships
User.hasMany(Post,   {as: 'posts',  foreignKey: 'userId'});
// creates instance methods:
// user.posts(conds)
// user.posts.build(data) // like new Post({userId: user.id});
// user.posts.create(data) // build and save

Post.belongsTo(User, {as: 'author', foreignKey: 'userId'});
// creates instance methods:
// post.author(callback) -- getter when called with function
// post.author() -- sync getter when called without params
// post.author(user) -- setter when called with object
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.defineProperty"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>defineProperty (prop, params)](#apidoc.element.jugglingdb.AbstractClass.defineProperty)
- description and source-code
```javascript
defineProperty = function (prop, params) {
    this.schema.defineProperty(this.modelName, prop, params);
}
```
- example usage
```shell
...
var list = this;
if (!(list instanceof List)) {
    return new List(data);
}

if (data && data instanceof List) data = data.items;

Object.defineProperty(list, 'parent', {
    writable: false,
    enumerable: false,
    configurable: false,
    value: parent
});

Object.defineProperty(list, 'nextid', {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.destroyAll"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>destroyAll ()](#apidoc.element.jugglingdb.AbstractClass.destroyAll)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
Post.update([{ where:{id:'1'}, update:{ published:false }},{ where:{id:'2'}, update:{ published:true }}], cb);
'''

SEE [model(3)](http://jugglingdb.co/model.3.html) for more information about
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.exists"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>exists ()](#apidoc.element.jugglingdb.AbstractClass.exists)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.find"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>find ()](#apidoc.element.jugglingdb.AbstractClass.find)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// get one latest post
Post.findOne({where: {published: true}, order: 'date DESC'}, cb);
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.findOne"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>findOne ()](#apidoc.element.jugglingdb.AbstractClass.findOne)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// all posts
Post.all(cb)
// all posts by user
Post.all({where: {userId: user.id}, order: 'id', limit: 10, skip: 20}, cb);
// the same as prev
user.posts(cb)
// get one latest post
Post.findOne({where: {published: true}, order: 'date DESC'}, cb);
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.findOrCreate"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>findOrCreate (query, data, callback)](#apidoc.element.jugglingdb.AbstractClass.findOrCreate)
- description and source-code
```javascript
function findOrCreate(query, data, callback) {
    if (typeof query === 'undefined') {
        query = {where: {}};
    }
    if (typeof data === 'function' || typeof data === 'undefined') {
        callback = data;
        data = query && query.where;
    }
    if (typeof callback === 'undefined') {
        callback = function () {};
    }

    var t = this;
    this.findOne(query, function (err, record) {
        if (err) return callback(err);
        if (record) return callback(null, record);
        t.create(data, callback);
    });
}
```
- example usage
```shell
...
        data = {};
    }
    var query = {};
    query[fk] = this.id;
    data[params.through.relationNameFor(fk)] = this;
    query[fk2] = acInst.id || acInst;
    data[params.through.relationNameFor(fk2)] = acInst;
    params.through.findOrCreate({where: query}, data, done);
};
scopeMethods.remove = function(acInst, done) {
    var q = {};
    q[fk] = this.id;
    q[fk2] = acInst.id || acInst;
    params.through.findOne({where: q}, function(err, d) {
        if (err) {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.hasAndBelongsToMany"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>hasAndBelongsToMany (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.hasAndBelongsToMany)
- description and source-code
```javascript
function hasAndBelongsToMany(anotherClass, params) {
    params = params || {};
    var models = this.schema.models;

    if ('string' === typeof anotherClass) {
        params.as = anotherClass;
        if (params.model) {
            anotherClass = params.model;
        } else {
            anotherClass = lookupModel(i8n.singularize(anotherClass)) ||
                anotherClass;
        }
        if (typeof anotherClass === 'string') {
            throw new Error('Could not find "' + anotherClass + '" relation for ' + this.modelName);
        }
    }

    if (!params.through) {
        var name1 = this.modelName + anotherClass.modelName;
        var name2 = anotherClass.modelName + this.modelName;
        params.through = lookupModel(name1) || lookupModel(name2) ||
            this.schema.define(name1);
    }
    params.through.belongsTo(this);
    params.through.belongsTo(anotherClass);

    this.hasMany(anotherClass, {as: params.as, through: params.through});

    function lookupModel(modelName) {
        var lookupClassName = modelName.toLowerCase();
        for (var name in models) {
            if (name.toLowerCase() === lookupClassName) {
                return models[name];
            }
        }
    }

}
```
- example usage
```shell
...

Post.belongsTo(User, {as: 'author', foreignKey: 'userId'});
// creates instance methods:
// post.author(callback) -- getter when called with function
// post.author() -- sync getter when called without params
// post.author(user) -- setter when called with object

User.hasAndBelongsToMany('groups');
// user.groups(callback) - get groups of user
// user.groups.create(data, callback) - create new group and connect with user
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.hasMany"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>hasMany (anotherClass, params)](#apidoc.element.jugglingdb.AbstractClass.hasMany)
- description and source-code
```javascript
function hasMany(anotherClass, params) {
    var thisClass = this, thisClassName = this.modelName;
    params = params || {};
    if (typeof anotherClass === 'string') {
        params.as = anotherClass;
        if (params.model) {
            anotherClass = params.model;
        } else {
            var anotherClassName = i8n.singularize(anotherClass).toLowerCase();
            for(var name in this.schema.models) {
                if (name.toLowerCase() === anotherClassName) {
                    anotherClass = this.schema.models[name];
                }
            }
        }
    }
    var methodName = params.as ||
        i8n.camelize(i8n.pluralize(anotherClass.modelName), true);
    var fk = params.foreignKey || i8n.camelize(thisClassName + '_id', true);

    this.relations[methodName] = {
        type: 'hasMany',
        keyFrom: 'id',
        keyTo: fk,
        modelTo: anotherClass,
        multiple: true
    };
    // each instance of this class should have method named
    // pluralize(anotherClass.modelName)
    // which is actually just anotherClass.all({where: {thisModelNameId: this.id}}, cb);
    var scopeMethods = {
        find: find,
        destroy: destroy
    };
    if (params.through) {

        // Append through relation, like modelTo
        this.relations[methodName].modelThrough = params.through;

        var fk2 = i8n.camelize(anotherClass.modelName + '_id', true);
        scopeMethods.create = function create(data, done) {
            if (typeof data !== 'object') {
                done = data;
                data = {};
            }
            if ('function' !== typeof done) {
                done = function() {};
            }
            var self = this;
            var id = this.id;
            anotherClass.create(data, function(err, ac) {
                if (err) return done(err, ac);
                var d = {};
                d[params.through.relationNameFor(fk)] = self;
                d[params.through.relationNameFor(fk2)] = ac;
                params.through.create(d, function(e) {
                    if (e) {
                        ac.destroy(function() {
                            done(e);
                        });
                    } else {
                        done(err, ac);
                    }
                });
            });
        };
        scopeMethods.add = function(acInst, data, done) {
            if (typeof data === 'function') {
                done = data;
                data = {};
            }
            var query = {};
            query[fk] = this.id;
            data[params.through.relationNameFor(fk)] = this;
            query[fk2] = acInst.id || acInst;
            data[params.through.relationNameFor(fk2)] = acInst;
            params.through.findOrCreate({where: query}, data, done);
        };
        scopeMethods.remove = function(acInst, done) {
            var q = {};
            q[fk] = this.id;
            q[fk2] = acInst.id || acInst;
            params.through.findOne({where: q}, function(err, d) {
                if (err) {
                    return done(err);
                }
                if (!d) {
                    return done();
                }
                d.destroy(done);
            });
        };
        delete scopeMethods.destroy;
    }
    defineScope(this.prototype, params.through || anotherClass, methodName, function () {
        var filter = {};
        filter.where = {};
        filter.where[fk] = this.id;
        if (params.through) {
            filter.collect = i8n.camelize(anotherClass.modelName, true);
            filter.include = filter.collect;
        }
        return filter;
    }, scopeMethods);

    if (!params.through) {
        // obviously, anotherClass should have attribute called 'fk'
        anotherClass.schema.defineForeignKey(anotherClass.modelName, fk, this.modelName);
    }

    function find(id, cb) {
        anotherClass.find(id, function (err, inst) {
            if (err) return cb(err);
            if (!inst) return cb(new Error('Not found'));
            if (inst[fk] && inst[fk].toStri ...
```
- example usage
```shell
...
schema.models.Post;
'''

SEE [schema(3)](http://jugglingdb.co/schema.3.html) for details schema usage.

'''javascript
// setup relationships
User.hasMany(Post,   {as: 'posts',  foreignKey: 'userId'});
// creates instance methods:
// user.posts(conds)
// user.posts.build(data) // like new Post({userId: user.id});
// user.posts.create(data) // build and save

Post.belongsTo(User, {as: 'author', foreignKey: 'userId'});
// creates instance methods:
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.include"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>include (objects, include, cb)](#apidoc.element.jugglingdb.AbstractClass.include)
- description and source-code
```javascript
include = function (objects, include, cb) {

    if ((include.constructor.name == 'Array' && include.length === 0) || (include.constructor.name == 'Object' && Object.keys(include
).length === 0)) {
        cb(null, objects);
        return;
    }

    include = processIncludeJoin(include);

    var keyVals = {};
    var objsByKeys = {};

    var nbCallbacks = 0;
    var totalCallbacks = 0;

    for (var i = 0; i < include.length; i++) {
        var callback = processIncludeItem(this, objects, include[i], keyVals, objsByKeys);
        if (callback !== null) {
            totalCallbacks++;
            if (callback instanceof Error) {
                cb(callback);
            } else {
                includeItemCallback(callback);
            }
        }
    }

    if (totalCallbacks === 0) {
        cb(null, objects);
    }

    function includeItemCallback(itemCb) {
        nbCallbacks++;
        itemCb(function () {
            nbCallbacks--;
            if (nbCallbacks === 0) {
                cb(null, objects);
            }
        });
    }

    function processIncludeJoin(ij) {
        if (typeof ij === 'string') {
            ij = [ij];
        }
        if (ij.constructor.name === 'Object') {
            var newIj = [];
            for (var key in ij) {
                var obj = {};
                obj[key] = ij[key];
                newIj.push(obj);
            }
            return newIj;
        }
        return ij;
    }
}
```
- example usage
```shell
...
*
* @param {Array} objects - array of instances
* @param {String}, {Object} or {Array} include - which relations you want to load.
* @param {Function} cb - Callback called when relations are loaded
*
* Examples:
*
* - User.include(users, 'posts', function() {}); will load all users posts with only one additional request.
* - User.include(users, ['posts'], function() {}); // same
* - User.include(users, ['posts', 'passports'], function() {}); // will load all users posts and passports with two
*     additional requests.
* - Passport.include(passports, {owner: 'posts'}, function() {}); // will load all passports owner (users), and all
*     posts of each owner loaded
* - Passport.include(passports, {owner: ['posts', 'passports']}); // ...
* - Passport.include(passports, {owner: [{posts: 'images'}, 'passports']}); // ...
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.iterate"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>iterate (filter, iterator, callback)](#apidoc.element.jugglingdb.AbstractClass.iterate)
- description and source-code
```javascript
function map(filter, iterator, callback) {
    var Model = this;
    if ('function' === typeof filter) {
        if ('function' === typeof iterator) {
            callback = iterator;
        }
        iterator = filter;
        filter = {};
    }

    var concurrent = filter.concurrent;
    delete filter.concurrent;
    var limit = filter.limit;
    var batchSize = filter.limit = filter.batchSize || 1000;
    var batchNumber = filter.batchNumber || -1;

    nextBatch();

    function nextBatch() {
        // console.log(batchNumber);
        batchNumber += 1;
        filter.skip = filter.offset = batchNumber * batchSize;
        if (limit < batchSize) {
            if (limit <= 0) {
                return done();
            } else {
                filter.limit = limit;
            }
        }
        limit -= batchSize;
        Model.all(filter).then(function(collection) {
            if (collection.length === 0) {
                return done();
            }
            var i = 0, wait;
            if (concurrent) {
                wait = collection.length;
                collection.forEach(function(obj, i) {
                    iterator(obj, next, filter.offset + i);
                    obj = null;
                });
                collection = null;
            } else {
                nextItem();
            }
            function next() {
                if (--wait === 0) {
                    nextBatch();
                }
            }
            function nextItem(err) {
                if (err) {
                    return done(err);
                }
                var item = collection[i];
                if (i > collection.length - 1) {
                    return nextBatch();
                }
                i += 1;
                setImmediate(function() {
                    iterator(item, nextItem, filter.offset + i);
                });
            }
        }).catch(done);
    }

    function done(err) {
        if ('function' === typeof callback) {
            callback(err);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.relationNameFor"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>relationNameFor (foreignKey)](#apidoc.element.jugglingdb.AbstractClass.relationNameFor)
- description and source-code
```javascript
function relationNameFor(foreignKey) {
    for (var rel in this.relations) {
        if (this.relations[rel].type === 'belongsTo' && this.relations[rel].keyFrom === foreignKey) {
            return rel;
        }
    }
}
```
- example usage
```shell
...
    done = function() {};
}
var self = this;
var id = this.id;
anotherClass.create(data, function(err, ac) {
    if (err) return done(err, ac);
    var d = {};
    d[params.through.relationNameFor(fk)] = self;
    d[params.through.relationNameFor(fk2)] = ac;
    params.through.create(d, function(e) {
        if (e) {
            ac.destroy(function() {
                done(e);
            });
        } else {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.scope"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>scope (name, params)](#apidoc.element.jugglingdb.AbstractClass.scope)
- description and source-code
```javascript
scope = function (name, params) {
    defineScope(this, this, name, params);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.toString"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>toString ()](#apidoc.element.jugglingdb.AbstractClass.toString)
- description and source-code
```javascript
toString = function () {
    return '[Model ' + this.modelName + ']';
}
```
- example usage
```shell
...
} else if (existsSync(schemaFile + 'coffee')) {
    schemaFile += 'coffee';
} else {
    schemaFile = false;
}

if (schemaFile) {
    var code = fs.readFileSync(schemaFile).toString();
    if (schemaFile.match(/\.coffee$/)) {
        code = require('coffee-script').compile(code);
    }
    /*jshint evil: true */
    var fn = new Function('context', 'require', 'with(context){(function(){' + code + '})()}');
    fn(context, require);
}
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.update"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>update ()](#apidoc.element.jugglingdb.AbstractClass.update)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
Post.update([{ where:{id:'1'}, update:{ published:false }},{ where:{id:'2'}, update:{ published:true }}], cb);
'''

SEE [model(3)](http://jugglingdb.co/model.3.html) for more information about
jugglingdb Model API. Or 'man jugglingdb-model' in terminal.
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.updateOrCreate"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>updateOrCreate ()](#apidoc.element.jugglingdb.AbstractClass.updateOrCreate)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.upsert"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>upsert ()](#apidoc.element.jugglingdb.AbstractClass.upsert)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validate"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validate ()](#apidoc.element.jugglingdb.AbstractClass.validate)
- description and source-code
```javascript
validate = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...
/**
* Validate using custom validator
*
* Default error message: is invalid
*
* Example:
*
*     User.validate('name', customValidator, {message: 'Bad name'});
*     function customValidator(err) {
*         if (this.name === 'bad') err();
*     });
*     var user = new User({name: 'Peter'});
*     user.isValid(); // true
*     user.name = 'bad';
*     user.isValid(); // false
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validateAsync"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validateAsync ()](#apidoc.element.jugglingdb.AbstractClass.validateAsync)
- description and source-code
```javascript
validateAsync = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...
/**
* Validate using custom async validator
*
* Default error message: is invalid
*
* Example:
*
*     User.validateAsync('name', customValidator, {message: 'Bad name'});
*     function customValidator(err, done) {
*         process.nextTick(function () {
*             if (this.name === 'bad') err();
*             done();
*         });
*     });
*     var user = new User({name: 'Peter'});
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesExclusionOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesExclusionOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesExclusionOf)
- description and source-code
```javascript
validatesExclusionOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...

'''javascript

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
if (!valid) {
    user.errors // hash of errors {attr: [errmessage, errmessage, ...], attr: ...}
}
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesFormatOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesFormatOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesFormatOf)
- description and source-code
```javascript
validatesFormatOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesInclusionOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesInclusionOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesInclusionOf)
- description and source-code
```javascript
validatesInclusionOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...
jugglingdb Model API. Or 'man jugglingdb-model' in terminal.

'''javascript

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
if (!valid) {
    user.errors // hash of errors {attr: [errmessage, errmessage, ...], attr: ...}
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesLengthOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesLengthOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesLengthOf)
- description and source-code
```javascript
validatesLengthOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...
SEE [model(3)](http://jugglingdb.co/model.3.html) for more information about
jugglingdb Model API. Or 'man jugglingdb-model' in terminal.

'''javascript

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
if (!valid) {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesNumericalityOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesNumericalityOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesNumericalityOf)
- description and source-code
```javascript
validatesNumericalityOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...
'''javascript

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
    if (!valid) {
        user.errors // hash of errors {attr: [errmessage, errmessage, ...], attr: ...}
    }
})
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesPresenceOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesPresenceOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesPresenceOf)
- description and source-code
```javascript
validatesPresenceOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...

SEE [model(3)](http://jugglingdb.co/model.3.html) for more information about
jugglingdb Model API. Or 'man jugglingdb-model' in terminal.

'''javascript

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.validatesUniquenessOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>validatesUniquenessOf ()](#apidoc.element.jugglingdb.AbstractClass.validatesUniquenessOf)
- description and source-code
```javascript
validatesUniquenessOf = function () {
    configure(this, name, arguments, opts);
}
```
- example usage
```shell
...

// Setup validations
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
    if (!valid) {
        user.errors // hash of errors {attr: [errmessage, errmessage, ...], attr: ...}
    }
})
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.whatTypeName"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.</span>whatTypeName (propName)](#apidoc.element.jugglingdb.AbstractClass.whatTypeName)
- description and source-code
```javascript
whatTypeName = function (propName) {
    var prop = this.schema.definitions[this.modelName].properties[propName];
    if (!prop || !prop.type) {
        return null;
        // throw new Error('Undefined type for ' + this.modelName + ':' + propName);
    }
    return prop.type.name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.AbstractClass.prototype"></a>[module jugglingdb.AbstractClass.prototype](#apidoc.module.jugglingdb.AbstractClass.prototype)

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype._adapter"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>_adapter ()](#apidoc.element.jugglingdb.AbstractClass.prototype._adapter)
- description and source-code
```javascript
_adapter = function () {
    return this.schema.adapter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype._initProperties"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>_initProperties (data, applySetters)](#apidoc.element.jugglingdb.AbstractClass.prototype._initProperties)
- description and source-code
```javascript
_initProperties = function (data, applySetters) {
    var self = this;
    var ctor = this.constructor;
    var ds = ctor.schema.definitions[ctor.modelName];
    var properties = ds.properties;
    data = data || {};

    Object.defineProperty(this, '__cachedRelations', {
        writable: true,
        enumerable: false,
        configurable: true,
        value: {}
    });

    Object.defineProperty(this, '__data', {
        writable: true,
        enumerable: false,
        configurable: true,
        value: {}
    });

    Object.defineProperty(this, '__dataWas', {
        writable: true,
        enumerable: false,
        configurable: true,
        value: {}
    });

    if (data.__cachedRelations) {
        this.__cachedRelations = data.__cachedRelations;
    }

    for (var i in data) {
        if (i in properties) {
            this.__data[i] = this.__dataWas[i] = data[i];
        } else if (i in ctor.relations) {
            this.__data[ctor.relations[i].keyFrom] = this.__dataWas[i] = data[i][ctor.relations[i].keyTo];
            this.__cachedRelations[i] = data[i];
        }
    }

    if (applySetters === true) {
        Object.keys(data).forEach(function (attr) {
            self[attr] = data[attr];
        });
    }

    ctor.forEachProperty(function (attr) {

        if ('undefined' === typeof self.__data[attr]) {
            self.__data[attr] = self.__dataWas[attr] = getDefault(attr);
        } else {
            self.__dataWas[attr] = self.__data[attr];
        }

    });

    ctor.forEachProperty(function (attr) {

        var type = properties[attr].type;

        if (BASE_TYPES.indexOf(type.name) === -1) {
            if (typeof self.__data[attr] !== 'object' && self.__data[attr]) {
                try {
                    self.__data[attr] = JSON.parse(self.__data[attr] + '');
                } catch (e) {
                    self.__data[attr] = String(self.__data[attr]);
                }
            }
            if (type.name === 'Array' || typeof type === 'object' && type.constructor.name === 'Array') {
                self.__data[attr] = new List(self.__data[attr], type, self);
            }
        }

    });

    function getDefault(attr) {
        var def = properties[attr]['default'];
        if (isdef(def)) {
            if (typeof def === 'function') {
                return def();
            } else {
                return def;
            }
        } else {
            return undefined;
        }
    }

    this.trigger('initialize');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>destroy ()](#apidoc.element.jugglingdb.AbstractClass.prototype.destroy)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
Post.update([{ where:{id:'1'}, update:{ published:false }},{ where:{id:'2'}, update:{ published:true }}], cb);
'''
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.fromObject"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>fromObject (obj)](#apidoc.element.jugglingdb.AbstractClass.prototype.fromObject)
- description and source-code
```javascript
fromObject = function (obj) {
    Object.keys(obj).forEach(function (key) {
        this[key] = obj[key];
    }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.inspect"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>inspect ()](#apidoc.element.jugglingdb.AbstractClass.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
    return util.inspect(this.__data, false, 4, true);
}
```
- example usage
```shell
...
    });

    return list;

}

List.prototype.inspect = function() {
    return util.inspect(this.items);
};

var _;
try {
    var underscore = 'underscore';
    _ = require(underscore);
} catch (e) {
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.isNewRecord"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>isNewRecord ()](#apidoc.element.jugglingdb.AbstractClass.prototype.isNewRecord)
- description and source-code
```javascript
isNewRecord = function () {
    return !this.id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.isValid"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>isValid (callback, data)](#apidoc.element.jugglingdb.AbstractClass.prototype.isValid)
- description and source-code
```javascript
isValid = function (callback, data) {
    var valid = true, inst = this, wait = 0, async = false;

    callback = callback || NOOP;

    // callback only needs one arguments, then the signature is 'callback(valid)'
    // convert it to standard node.js callback style
    if (callback.length < 2) {
        var _callback = callback;
        callback = function (err, valid) {
            _callback(valid);
        };
    }

    // exit with success when no errors
    if (!this.constructor._validations) {
        cleanErrors(this);
        if (callback) {
            this.trigger('validate', function(validationsDone) {
                validationsDone.call(inst, function() {
                    callback(null, valid);
                });
            }, data, function (err) {
                callback(err, false);
            });
        }
        return valid;
    }

    Object.defineProperty(this, 'errors', {
        enumerable: false,
        configurable: true,
        value: new Errors(this)
    });

    this.trigger('validate', function (validationsDone) {
        var inst = this,
            asyncFail = false;

        this.constructor._validations.forEach(function (v) {
            if (v[2] && v[2].async) {
                async = true;
                wait += 1;
                process.nextTick(function () {
                    validationFailed(inst, v, done);
                });
            } else {
                if (validationFailed(inst, v)) {
                    valid = false;
                }
            }

        });

        if (!async) {
            validationsDone.call(inst, function() {
                if (valid) cleanErrors(inst);
                if (callback) {
                    callback(valid ? null : new ValidationError(this), valid);
                }
            });
        }

        function done(fail) {
            asyncFail = asyncFail || fail;
            if (--wait === 0) {
                validationsDone.call(inst, function () {
                    if (valid && !asyncFail) cleanErrors(inst);
                    if (callback) {
                        callback(valid ? null : new ValidationError(this), valid && !asyncFail);
                    }
                });
            }
        }

    }, data, function (err) {
        callback(err, false);
    });

    if (async) {
        // in case of async validation we should return undefined here,
        // because not all validations are finished yet
        return;
    } else {
        return valid;
    }

}
```
- example usage
```shell
...
User.validatesPresenceOf('name', 'email')
User.validatesLengthOf('password', {min: 5, message: {min: 'Password is too short'}});
User.validatesInclusionOf('gender', {in: ['male', 'female']});
User.validatesExclusionOf('domain', {in: ['www', 'billing', 'admin']});
User.validatesNumericalityOf('age', {int: true});
User.validatesUniquenessOf('email', {message: 'email is not unique'});

user.isValid(function (valid) {
    if (!valid) {
        user.errors // hash of errors {attr: [errmessage, errmessage, ...], attr: ...}
    }
})

'''
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.propertyChanged"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>propertyChanged (attr)](#apidoc.element.jugglingdb.AbstractClass.prototype.propertyChanged)
- description and source-code
```javascript
function propertyChanged(attr) {
    return this.__data[attr] !== this.__dataWas[attr];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.reload"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>reload ()](#apidoc.element.jugglingdb.AbstractClass.prototype.reload)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.reset"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>reset ()](#apidoc.element.jugglingdb.AbstractClass.prototype.reset)
- description and source-code
```javascript
reset = function () {
    var obj = this;
    Object.keys(obj).forEach(function (k) {
        if (k !== 'id' && !obj.constructor.schema.definitions[obj.constructor.modelName].properties[k]) {
            delete obj[k];
        }
        if (obj.propertyChanged(k)) {
            obj[k] = obj[k + '_was'];
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.save"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>save ()](#apidoc.element.jugglingdb.AbstractClass.prototype.save)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables

// work with models:
var user = new User;
user.save(function (err) {
    var post = user.posts.build({title: 'Hello world'});
    post.save(console.log);
});

// or just call it as function (with the same result):
var user = User();
user.save(...);
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>toJSON ()](#apidoc.element.jugglingdb.AbstractClass.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    return this.toObject(false, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.toObject"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>toObject (onlySchema, cachedRelations)](#apidoc.element.jugglingdb.AbstractClass.prototype.toObject)
- description and source-code
```javascript
toObject = function (onlySchema, cachedRelations) {
    var data = {};
    var ds = this.constructor.schema.definitions[this.constructor.modelName];
    var properties = ds.properties;
    var self = this;

    this.constructor.forEachProperty(function (attr) {
        if (self[attr] instanceof List) {
            data[attr] = self[attr].toObject();
        } else if (self.__data.hasOwnProperty(attr)) {
            data[attr] = self[attr];
        } else {
            data[attr] = null;
        }
    });

    if (!onlySchema) {
        Object.keys(self).forEach(function (attr) {
            if (!data.hasOwnProperty(attr)) {
                data[attr] = self[attr];
            }
        });

        if (cachedRelations === true && this.__cachedRelations) {
            var relations = this.__cachedRelations;
            Object.keys(relations).forEach(function (attr) {
                if (!data.hasOwnProperty(attr)) {
                    data[attr] = relations[attr];
                }
            });
        }
    }

    return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.trigger"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>trigger (actionName, work, data, quit)](#apidoc.element.jugglingdb.AbstractClass.prototype.trigger)
- description and source-code
```javascript
function trigger(actionName, work, data, quit) {
    var capitalizedName = capitalize(actionName);
    var beforeHook = this.constructor["before" + capitalizedName];
    var afterHook = this.constructor["after" + capitalizedName];
    if (actionName === 'validate') {
        beforeHook = beforeHook || this.constructor.beforeValidation;
        afterHook = afterHook || this.constructor.afterValidation;
    }
    var inst = this;

    // we only call "before" hook when we have actual action (work) to perform
    if (work) {
        if (beforeHook) {
            // before hook should be called on instance with one param: callback
            beforeHook.call(inst, function (err) {
                if (err) {
                    if (quit) {
                        quit.call(inst, err);
                    }
                    return;
                }
                // actual action also have one param: callback
                work.call(inst, next);
            }, data);
        } else {
            work.call(inst, next);
        }
    } else {
        next();
    }

    function next(done) {
        if (afterHook) {
            afterHook.call(inst, done);
        } else if (done) {
            done.call(this);
        }
    }
}
```
- example usage
```shell
...
    };
}

// exit with success when no errors
if (!this.constructor._validations) {
    cleanErrors(this);
    if (callback) {
        this.trigger('validate', function(validationsDone) {
            validationsDone.call(inst, function() {
                callback(null, valid);
            });
        }, data, function (err) {
            callback(err, false);
        });
    }
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.updateAttribute"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>updateAttribute ()](#apidoc.element.jugglingdb.AbstractClass.prototype.updateAttribute)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
...
// beforeValidate
// afterValidate
// beforeSave
// beforeUpdate
// afterUpdate
// afterSave
// callback
user.updateAttribute('email', 'email@example.com', callback);
// beforeValidate
// afterValidate
// beforeSave
// beforeUpdate
// afterUpdate
// afterSave
// callback
...
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.updateAttributes"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>updateAttributes ()](#apidoc.element.jugglingdb.AbstractClass.prototype.updateAttributes)
- description and source-code
```javascript
function promisedWrap() {
    var args = [].slice.call(arguments);
    var callback = 'function' === typeof args[args.length - 1] ? args.pop() : null;
    var self = this;
    var Model = isClassMethod ? self : self.constructor;
    var queryResult;
    var promisedQuery = connection(Model.schema)
    .then(function() {
        return new when.Promise(function(resolve, reject) {
            args.push(function(err, result) {
                queryResult = result;
                if (err) {
                    reject(err);
                } else {
                    resolve(result);
                }
            });
            fn.apply(self, args);
        });
    });
    if (callback) {
        promisedQuery.then(function(result) {
            callback(null, result);
        }, function(err) {
            if ('undefined' !== queryResult) {
                callback(err, queryResult);
            } else {
                callback(err);
            }
        });
    } else {
        return promisedQuery;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.AbstractClass.prototype.whatTypeName"></a>[function <span class="apidocSignatureSpan">jugglingdb.AbstractClass.prototype.</span>whatTypeName (propName)](#apidoc.element.jugglingdb.AbstractClass.prototype.whatTypeName)
- description and source-code
```javascript
whatTypeName = function (propName) {
    return this.constructor.whatTypeName(propName);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.BaseSQL"></a>[module jugglingdb.BaseSQL](#apidoc.module.jugglingdb.BaseSQL)

#### <a name="apidoc.element.jugglingdb.BaseSQL.BaseSQL"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>BaseSQL ()](#apidoc.element.jugglingdb.BaseSQL.BaseSQL)
- description and source-code
```javascript
function BaseSQL() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.BaseSQL.prototype"></a>[module jugglingdb.BaseSQL.prototype](#apidoc.module.jugglingdb.BaseSQL.prototype)

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.automigrate"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>automigrate (cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.automigrate)
- description and source-code
```javascript
automigrate = function (cb) {
    var self = this;
    var wait = 0;
    Object.keys(this._models).forEach(function (model) {
        wait += 1;
        self.dropTable(model, function () {
            // console.log('drop', model);
            self.createTable(model, function (err) {
                // console.log('create', model);
                if (err) console.log(err);
                done();
            });
        });
    });
    if (wait === 0) cb();

    function done() {
        if (--wait === 0 && cb) {
            cb();
        }
    }
}
```
- example usage
```shell
...

User.hasAndBelongsToMany('groups');
// user.groups(callback) - get groups of user
// user.groups.create(data, callback) - create new group and connect with user
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables

// work with models:
var user = new User;
user.save(function (err) {
    var post = user.posts.build({title: 'Hello world'});
    post.save(console.log);
});
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.command"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>command (sql, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.command)
- description and source-code
```javascript
command = function (sql, callback) {
    return this.query(sql, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.count"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>count (model, callback, where)](#apidoc.element.jugglingdb.BaseSQL.prototype.count)
- description and source-code
```javascript
function count(model, callback, where) {
    var self = this;
    var props = this._models[model].properties;

    this.queryOne('SELECT count(*) as cnt FROM ' +
        this.tableEscaped(model) + ' ' + buildWhere(where), function (err, res) {
        if (err) return callback(err);
        callback(err, res && res.cnt);
    });

    function buildWhere(conds) {
        var cs = [];
        Object.keys(conds || {}).forEach(function (key) {
            var keyEscaped = self.escapeName(key);
            if (conds[key] === null) {
                cs.push(keyEscaped + ' IS NULL');
            } else {
                cs.push(keyEscaped + ' = ' + self.toDatabase(props[key], conds[key]));
            }
        });
        return cs.length ? ' WHERE ' + cs.join(' AND ') : '';
    }
}
```
- example usage
```shell
...
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.createTable"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>createTable (model, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.createTable)
- description and source-code
```javascript
createTable = function (model, cb) {
    this.command('CREATE TABLE ' + this.tableEscaped(model) +
        ' (\n  ' + this.propertiesSQL(model) + '\n)', cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.define"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>define (descr)](#apidoc.element.jugglingdb.BaseSQL.prototype.define)
- description and source-code
```javascript
define = function (descr) {
    if (!descr.settings) descr.settings = {};
    this._models[descr.model.modelName] = descr;
}
```
- example usage
```shell
...

## Usage

'''javascript
var Schema = require('jugglingdb').Schema;
var schema = new Schema('redis', {port: 6379}); //port number depends on your configuration
// define models
var Post = schema.define('Post', {
    title:     { type: String, length: 255 },
    content:   { type: Schema.Text },
    date:      { type: Date,    default: function () { return new Date;} },
    timestamp: { type: Number,  default: Date.now },
    published: { type: Boolean, default: false, index: true }
});
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.defineProperty"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>defineProperty (model, prop, params)](#apidoc.element.jugglingdb.BaseSQL.prototype.defineProperty)
- description and source-code
```javascript
defineProperty = function (model, prop, params) {
    this._models[model].properties[prop] = params;
}
```
- example usage
```shell
...
var list = this;
if (!(list instanceof List)) {
    return new List(data);
}

if (data && data instanceof List) data = data.items;

Object.defineProperty(list, 'parent', {
    writable: false,
    enumerable: false,
    configurable: false,
    value: parent
});

Object.defineProperty(list, 'nextid', {
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>destroy (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.destroy)
- description and source-code
```javascript
function destroy(model, id, callback) {
    var sql = 'DELETE FROM ' +
        this.tableEscaped(model) + ' WHERE ' + this.escapeName('id') + ' = ' + this.escapeId(id);

    this.command(sql, function (err) {
        callback(err);
    });
}
```
- example usage
```shell
...
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
Post.update([{ where:{id:'1'}, update:{ published:false }},{ where:{id:'2'}, update:{ published:true }}], cb);
'''
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.destroyAll"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>destroyAll (model, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.destroyAll)
- description and source-code
```javascript
function destroyAll(model, callback) {
    this.command('DELETE FROM ' + this.tableEscaped(model), function (err) {
        if (err) {
            return callback(err, []);
        }
        callback(err);
    }.bind(this));
}
```
- example usage
```shell
...
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
Post.update({ where:{id:'1'}, update:{ published:false }}, cb);
// update bulk posts (currently only on the mysql adapter)
Post.update([{ where:{id:'1'}, update:{ published:false }},{ where:{id:'2'}, update:{ published:true }}], cb);
'''

SEE [model(3)](http://jugglingdb.co/model.3.html) for more information about
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>disconnect ()](#apidoc.element.jugglingdb.BaseSQL.prototype.disconnect)
- description and source-code
```javascript
function disconnect() {
    this.client.end();
}
```
- example usage
```shell
...

/**
 * Close database connection
 */
Schema.prototype.disconnect = function disconnect(cb) {
    if (typeof this.adapter.disconnect === 'function') {
        this.connected = false;
        this.adapter.disconnect(cb);
        this.emit('disconnected');
    } else if (cb) {
        cb();
    }
};

Schema.prototype.copyModel = function copyModel(Master) {
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.dropTable"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>dropTable (model, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.dropTable)
- description and source-code
```javascript
dropTable = function (model, cb) {
    this.command('DROP TABLE IF EXISTS ' + this.tableEscaped(model), cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.escapeId"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>escapeId (id)](#apidoc.element.jugglingdb.BaseSQL.prototype.escapeId)
- description and source-code
```javascript
escapeId = function (id) {
    if (this.schema.settings.slave) {
        if (null === id) {
            return 'NULL';
        }
        return '"' + ('undefined' === typeof id ? '' : id.toString().replace(/["\n]/g, '')) + '"';
    } else {
        var idNumber = Number(id);
        if (isNaN(idNumber)) {
            throw new Error('id is not a number');
        }
        return idNumber;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.escapeName"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>escapeName (name)](#apidoc.element.jugglingdb.BaseSQL.prototype.escapeName)
- description and source-code
```javascript
escapeName = function (name) {
    throw new Error('escapeName method should be declared in adapter');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.exists"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>exists (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.exists)
- description and source-code
```javascript
exists = function (model, id, callback) {
    var sql = 'SELECT 1 FROM ' +
        this.tableEscaped(model) + ' WHERE ' + this.escapeName('id') + ' = ' + this.escapeId(id) + ' LIMIT 1';

    this.query(sql, function (err, data) {
        if (err) return callback(err);
        callback(null, data.length === 1);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.find"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>find (model, id, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.find)
- description and source-code
```javascript
function find(model, id, callback) {
    var idNumber = this.escapeId(id);
    var sql = 'SELECT * FROM ' +
        this.tableEscaped(model) + ' WHERE ' + this.escapeName('id') + ' = ' + idNumber + ' LIMIT 1';

    this.query(sql, function (err, data) {
        if (data && data.length === 1) {
            data[0].id = id;
        } else {
            data = [null];
        }
        callback(err, this.fromDatabase(model, data[0]));
    }.bind(this));
}
```
- example usage
```shell
...
// get one latest post
Post.findOne({where: {published: true}, order: 'date DESC'}, cb);
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.query"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>query ()](#apidoc.element.jugglingdb.BaseSQL.prototype.query)
- description and source-code
```javascript
query = function () {
    throw new Error('query method should be declared in adapter');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.queryOne"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>queryOne (sql, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.queryOne)
- description and source-code
```javascript
queryOne = function (sql, callback) {
    return this.query(sql, function (err, data) {
        if (err) return callback(err);
        callback(err, data[0]);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.save"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>save (model, data, callback)](#apidoc.element.jugglingdb.BaseSQL.prototype.save)
- description and source-code
```javascript
save = function (model, data, callback) {
    var sql = 'UPDATE ' + this.tableEscaped(model) + ' SET ' + this.toFields(model, data) + ' WHERE ' + this.escapeName('id') + ' = ' +
this.escapeId(data.id);

    this.query(sql, function (err) {
        callback(err);
    });
}
```
- example usage
```shell
...
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables

// work with models:
var user = new User;
user.save(function (err) {
    var post = user.posts.build({title: 'Hello world'});
    post.save(console.log);
});

// or just call it as function (with the same result):
var user = User();
user.save(...);
...
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.table"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>table (model)](#apidoc.element.jugglingdb.BaseSQL.prototype.table)
- description and source-code
```javascript
table = function (model) {
    return this._models[model].model.tableName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.tableEscaped"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>tableEscaped (model)](#apidoc.element.jugglingdb.BaseSQL.prototype.tableEscaped)
- description and source-code
```javascript
tableEscaped = function (model) {
    return this.escapeName(this.table(model));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.BaseSQL.prototype.updateAttributes"></a>[function <span class="apidocSignatureSpan">jugglingdb.BaseSQL.prototype.</span>updateAttributes (model, id, data, cb)](#apidoc.element.jugglingdb.BaseSQL.prototype.updateAttributes)
- description and source-code
```javascript
function updateAttrs(model, id, data, cb) {
    data.id = id;
    this.save(model, data, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.Schema"></a>[module jugglingdb.Schema](#apidoc.module.jugglingdb.Schema)

#### <a name="apidoc.element.jugglingdb.Schema.Schema"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>Schema (name, settings)](#apidoc.element.jugglingdb.Schema.Schema)
- description and source-code
```javascript
function Schema(name, settings) {
    var schema = this;
    // just save everything we get
    this.name = name;
    this.settings = settings || {};

    // Disconnected by default
    this.connected = false;
    this.connecting = false;

    // create blank models pool
    this.models = {};
    this.definitions = {};

    if (this.settings.log) {
        this.on('log', function(str, duration) {
            console.log(str);
        });
    }

    // and initialize schema using adapter
    // this is only one initialization entry point of adapter
    // this module should define 'adapter' member of 'this' (schema)
    var adapter;
    if (typeof name === 'object') {
        adapter = name;
        this.name = adapter.name;
    } else if (name.match(/^\//)) {
        // try absolute path
        adapter = require(name);
    } else if (existsSync(__dirname + '/adapters/' + name + '.js')) {
        // try built-in adapter
        adapter = require('./adapters/' + name);
    } else {
        // try foreign adapter
        try {
            adapter = require('jugglingdb-' + name);
        } catch (e) {
            return console.log('\nWARNING: JugglingDB adapter "' + name + '" is not installed,\nso your models would not work, to
 fix run:\n\n    npm install jugglingdb-' + name, '\n');
        }
    }

    this.connecting = true;
    adapter.initialize(this, function () {

        this.adapter.log = function (query, start) {
            schema.log(query, start);
        };

        this.adapter.logger = function (query) {
            var t1 = Date.now();
            var log = this.log;
            return function (q) {
                log(q || query, t1);
            };
        };

        this.connecting = false;
        this.connected = true;
        this.emit('connected');

    }.bind(this));

    // we have an adaper now?
    if (!this.adapter) {
        this.emit('disconnected');
        throw new Error('Adapter "' + name + '" is not defined correctly: it should define 'adapter' member of schema synchronously
');
    }

    schema.connect = function(cb) {
        var schema = this;
        schema.connecting = true;
        return new when.Promise(function(resolve, reject) {
            if (!schema.adapter.connect) {
                return process.nextTick(function() {
                    schema.connecting = false;
                    if (cb) {
                        cb(null, schema);
                    }
                    return resolve(schema);
                });
            }
            schema.adapter.connect(function(err) {
                if (err) {
                    schema.connected = false;
                    schema.connecting = false;
                    reject(err);
                    if (cb) {
                        cb(err);
                    }
                } else {
                    schema.connected = true;
                    schema.connecting = false;
                    schema.emit('connected');
                    resolve(schema);
                    if (cb) {
                        cb(null, schema);
                    }
                }
            });
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.JSON"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>JSON ()](#apidoc.element.jugglingdb.Schema.JSON)
- description and source-code
```javascript
function JSON() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.Text"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>Text (s)](#apidoc.element.jugglingdb.Schema.Text)
- description and source-code
```javascript
function Text(s) { return s; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.registerType"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>registerType (type)](#apidoc.element.jugglingdb.Schema.registerType)
- description and source-code
```javascript
registerType = function (type) {
    this.types[type.name] = type;
}
```
- example usage
```shell
...
Schema.JSON = function JSON() {};

Schema.types = {};
Schema.registerType = function (type) {
   this.types[type.name] = type;
};

Schema.registerType(Schema.Text);
Schema.registerType(Schema.JSON);


/**
* Schema - adapter-specific classes factory.
*
* All classes in single schema shares same adapter type and
...
```

#### <a name="apidoc.element.jugglingdb.Schema.super_"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.</span>super_ ()](#apidoc.element.jugglingdb.Schema.super_)
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



# <a name="apidoc.module.jugglingdb.Schema.prototype"></a>[module jugglingdb.Schema.prototype](#apidoc.module.jugglingdb.Schema.prototype)

#### <a name="apidoc.element.jugglingdb.Schema.prototype.automigrate"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>automigrate (cb)](#apidoc.element.jugglingdb.Schema.prototype.automigrate)
- description and source-code
```javascript
automigrate = function (cb) {
    this.freeze();
    if (this.adapter.automigrate) {
        this.adapter.automigrate(cb);
    } else if (cb) {
        cb();
    }
}
```
- example usage
```shell
...

User.hasAndBelongsToMany('groups');
// user.groups(callback) - get groups of user
// user.groups.create(data, callback) - create new group and connect with user
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables

// work with models:
var user = new User;
user.save(function (err) {
    var post = user.posts.build({title: 'Hello world'});
    post.save(console.log);
});
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.autoupdate"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>autoupdate (cb)](#apidoc.element.jugglingdb.Schema.prototype.autoupdate)
- description and source-code
```javascript
autoupdate = function (cb) {
    this.freeze();
    if (this.adapter.autoupdate) {
        this.adapter.autoupdate(cb);
    } else if (cb) {
        cb();
    }
}
```
- example usage
```shell
...
    compound.root + '/db/schema',
    compound.app.get('database'),
    compound
);
if (compound.app.enabled('autoupdate')) {
    compound.on('ready', function() {
        compound.orm.schema.forEach(function(s) {
            s.autoupdate();
            if (s.backyard) {
                s.backyard.autoupdate();
                s.backyard.log = s.log;
            }
        });
    });
}
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.copyModel"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>copyModel (Master)](#apidoc.element.jugglingdb.Schema.prototype.copyModel)
- description and source-code
```javascript
function copyModel(Master) {
    var schema = this;
    var className = Master.modelName;
    var md = Master.schema.definitions[className];
    var Slave = function SlaveModel() {
        Master.apply(this, [].slice.call(arguments));
        this.schema = schema;
    };

    util.inherits(Slave, Master);

    Slave.__proto__ = Master;

    hiddenProperty(Slave, 'schema', schema);
    hiddenProperty(Slave, 'modelName', className);
    hiddenProperty(Slave, 'tableName', Master.tableName);
    hiddenProperty(Slave, 'relations', Master.relations);

    if (!(className in schema.models)) {

        // store class in model pool
        schema.models[className] = Slave;
        schema.definitions[className] = {
            properties: md.properties,
            settings: md.settings
        };

        if (!schema.isTransaction) {
            schema.adapter.define({
                model:      Slave,
                properties: md.properties,
                settings:   md.settings
            });
        }

    }

    return Slave;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.define"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>define (className, properties, settings)](#apidoc.element.jugglingdb.Schema.prototype.define)
- description and source-code
```javascript
function defineClass(className, properties, settings) {
    var schema = this;
    var args = slice.call(arguments);

    if (!className) {
        throw new Error('Class name required');
    }
    if (args.length == 1) {
        properties = {};
        args.push(properties);
    }
    if (args.length == 2) {
        settings = {};
        args.push(settings);
    }

    settings = settings || {};

    if ('function' === typeof properties) {
        var props = {};
        properties({
            property: function(name, type, settings) {
                settings = settings || {};
                settings.type = type;
                props[name] = settings;
            },
            set: function(key, val) {
                settings[key] = val;
            }
        });
        properties = props;
    }

    properties = properties || {};

    // every class can receive hash of data as optional param
    var NewClass = function ModelConstructor(data, schema) {
        if (!(this instanceof ModelConstructor)) {
            return new ModelConstructor(data);
        }
        AbstractClass.call(this, data);
        hiddenProperty(this, 'schema', schema || this.constructor.schema);
    };

    hiddenProperty(NewClass, 'schema', schema);
    hiddenProperty(NewClass, 'settings', settings);
    hiddenProperty(NewClass, 'properties', properties);
    hiddenProperty(NewClass, 'modelName', className);
    hiddenProperty(NewClass, 'tableName', settings.table || className);
    hiddenProperty(NewClass, 'relations', {});

    // inherit AbstractClass methods
    for (var i in AbstractClass) {
        NewClass[i] = AbstractClass[i];
    }
    for (var j in AbstractClass.prototype) {
        NewClass.prototype[j] = AbstractClass.prototype[j];
    }

    NewClass.getter = {};
    NewClass.setter = {};

    standartize(properties, settings);

    // store class in model pool
    this.models[className] = NewClass;
    this.definitions[className] = {
        properties: properties,
        settings: settings
    };

    // pass control to adapter
    this.adapter.define({
        model:      NewClass,
        properties: properties,
        settings:   settings
    });

    NewClass.prototype.__defineGetter__('id', function () {
        return this.__data.id;
    });

    properties.id = properties.id || { type: schema.settings.slave ? String : Number };

    NewClass.forEachProperty = function (cb) {
        Object.keys(properties).forEach(cb);
    };

    NewClass.registerProperty = function (attr) {
        var DataType = properties[attr].type;
        if (DataType instanceof Array) {
            DataType = List;
        } else if (DataType.name === 'Date') {
            var OrigDate = Date;
            DataType = function Date(arg) {
                return new OrigDate(arg);
            };
        } else if (DataType.name === 'JSON' || DataType === JSON) {
            DataType = function JSON(s) {
                return s;
            };
        } else if (DataType.name === 'Text' || DataType === Schema.Text) {
            DataType = function Text(s) {
                return s;
            };
        }

        Object.defineProperty(NewClass.prototype, attr, {
            get: function () {
                if (NewClass.getter[attr]) {
                    return NewClass.getter[attr].call(this);
                } else {
                    return this.__data[attr];
                }
            },
            set: function (value) {
                if (NewClass.setter[attr]) {
                    NewClass.setter[attr].call(this, value);
                } else {
                    if (value === null || value === undefined || typeof DataType === 'object') {
                        this.__data[attr] = value;
                    } else if (DataType === Boolean) {
                        this.__data[attr] = value === 'false' ? false : !!value;
                    } else {
                        this.__data[attr] = DataType(value);
                    }
                }
            },
            configurable: true,
            enumera ...
```
- example usage
```shell
...

## Usage

'''javascript
var Schema = require('jugglingdb').Schema;
var schema = new Schema('redis', {port: 6379}); //port number depends on your configuration
// define models
var Post = schema.define('Post', {
    title:     { type: String, length: 255 },
    content:   { type: Schema.Text },
    date:      { type: Date,    default: function () { return new Date;} },
    timestamp: { type: Number,  default: Date.now },
    published: { type: Boolean, default: false, index: true }
});
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.defineForeignKey"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>defineForeignKey (className, key, foreignClassName)](#apidoc.element.jugglingdb.Schema.prototype.defineForeignKey)
- description and source-code
```javascript
function defineForeignKey(className, key, foreignClassName) {
    // quit if key already defined
    if (this.definitions[className].properties[key]) return;

    if (this.adapter.defineForeignKey) {
        var cb = function (err, keyType) {
            if (err) throw err;
            this.definitions[className].properties[key] = {type: keyType};
        }.bind(this);
        switch (this.adapter.defineForeignKey.length) {
            case 4:
                this.adapter.defineForeignKey(className, key, foreignClassName, cb);
            break;
            default:
            case 3:
                this.adapter.defineForeignKey(className, key, cb);
            break;
        }
    } else {
        this.definitions[className].properties[key] = {type: Number};
    }
    this.models[className].registerProperty(key);
}
```
- example usage
```shell
...
        filter.include = filter.collect;
    }
    return filter;
}, scopeMethods);

if (!params.through) {
    // obviously, anotherClass should have attribute called 'fk'
    anotherClass.schema.defineForeignKey(anotherClass.modelName, fk, this.modelName);
}

function find(id, cb) {
    anotherClass.find(id, function (err, inst) {
        if (err) return cb(err);
        if (!inst) return cb(new Error('Not found'));
        if (inst[fk] && inst[fk].toString() == this.id.toString()) {
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.defineProperty"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>defineProperty (model, prop, params)](#apidoc.element.jugglingdb.Schema.prototype.defineProperty)
- description and source-code
```javascript
defineProperty = function (model, prop, params) {
    this.definitions[model].properties[prop] = params;
    this.models[model].registerProperty(prop);
    if (this.adapter.defineProperty) {
        this.adapter.defineProperty(model, prop, params);
    }
}
```
- example usage
```shell
...
var list = this;
if (!(list instanceof List)) {
    return new List(data);
}

if (data && data instanceof List) data = data.items;

Object.defineProperty(list, 'parent', {
    writable: false,
    enumerable: false,
    configurable: false,
    value: parent
});

Object.defineProperty(list, 'nextid', {
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>disconnect (cb)](#apidoc.element.jugglingdb.Schema.prototype.disconnect)
- description and source-code
```javascript
function disconnect(cb) {
    if (typeof this.adapter.disconnect === 'function') {
        this.connected = false;
        this.adapter.disconnect(cb);
        this.emit('disconnected');
    } else if (cb) {
        cb();
    }
}
```
- example usage
```shell
...

/**
 * Close database connection
 */
Schema.prototype.disconnect = function disconnect(cb) {
    if (typeof this.adapter.disconnect === 'function') {
        this.connected = false;
        this.adapter.disconnect(cb);
        this.emit('disconnected');
    } else if (cb) {
        cb();
    }
};

Schema.prototype.copyModel = function copyModel(Master) {
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.extendModel"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>extendModel (model, props)](#apidoc.element.jugglingdb.Schema.prototype.extendModel)
- description and source-code
```javascript
extendModel = function (model, props) {
    var t = this;
    standartize(props, {});
    Object.keys(props).forEach(function (propName) {
        var definition = props[propName];
        t.defineProperty(model, propName, definition);
    });
}
```
- example usage
```shell
...
 *     // amend the content model with competition attributes
 *     db.defineProperty('Content', 'competitionType', { type: String });
 *     db.defineProperty('Content', 'expiryDate', { type: Date, index: true });
 *     db.defineProperty('Content', 'isExpired', { type: Boolean, index: true });
 *
 *     // schema.extend allows to
 *     // extend the content model with competition attributes
 *     db.extendModel('Content', {
 *       competitionType: String,
 *       expiryDate: { type: Date, index: true },
 *       isExpired: { type: Boolean, index: true }
 *     });
 */
Schema.prototype.extendModel = function (model, props) {
var t = this;
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.freeze"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>freeze ()](#apidoc.element.jugglingdb.Schema.prototype.freeze)
- description and source-code
```javascript
function freeze() {
    if (this.adapter.freezeSchema) {
        this.adapter.freezeSchema();
    }
}
```
- example usage
```shell
...
}

// autoupdate if set app.enable('autoupdate')  or freeze schemas by default
railway.orm._schemas.forEach(function (schema) {
    if(app.enabled('autoupdate')){
        schema.autoupdate();
    } else {
        schema.freeze();
    }
});
}

function log(str, startTime) {
var $ = railway.utils.stylize.$;
var m = Date.now() - startTime;
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.isActual"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>isActual (cb)](#apidoc.element.jugglingdb.Schema.prototype.isActual)
- description and source-code
```javascript
isActual = function (cb) {
    this.freeze();
    if (this.adapter.isActual) {
        this.adapter.isActual(cb);
    } else if (cb) {
        cb(null, true);
    }
}
```
- example usage
```shell
...
/**
* Check whether migrations needed
* This method make sense only for sql adapters.
*/
Schema.prototype.isActual = function (cb) {
   this.freeze();
   if (this.adapter.isActual) {
       this.adapter.isActual(cb);
   } else if (cb) {
       cb(null, true);
   }
};

/**
* Log benchmarked message. Do not redefine this method, if you need to grab
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.log"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>log (sql, t)](#apidoc.element.jugglingdb.Schema.prototype.log)
- description and source-code
```javascript
log = function (sql, t) {
    this.emit('log', sql, t);
}
```
- example usage
```shell
...

exports.loadSchema = function(filename, settings, compound) {
var schema = [];
var definitions = require(filename);
Object.keys(definitions).forEach(function(k) {
    var conf = settings[k];
    if (!conf) {
        console.log('No config found for ' + k + ' schema, using in-memory schema');
        conf = {driver: 'memory'};
    }
    schema[k] = new Schema(conf.driver, conf);
    schema[k].on('define', function(m, name, prop, sett) {
        compound.models[name] = m;
        if (conf.backyard) {
            schema[k].backyard.define(name, prop, sett);
...
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.tableName"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>tableName (modelName)](#apidoc.element.jugglingdb.Schema.prototype.tableName)
- description and source-code
```javascript
tableName = function (modelName) {
    return this.models[modelName].model.tableName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.prototype.transaction"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.prototype.</span>transaction ()](#apidoc.element.jugglingdb.Schema.prototype.transaction)
- description and source-code
```javascript
transaction = function () {
    var schema = this;
    var transaction = new EventEmitter();
    transaction.isTransaction = true;
    transaction.origin = schema;
    transaction.name = schema.name;
    transaction.settings = schema.settings;
    transaction.connected = false;
    transaction.connecting = false;
    transaction.adapter = schema.adapter.transaction();

    // create blank models pool
    transaction.models = {};
    transaction.definitions = {};

    for (var i in schema.models) {
        schema.copyModel.call(transaction, schema.models[i]);
    }

    transaction.connect = schema.connect;

    transaction.exec = function(cb) {
        transaction.adapter.exec(cb);
    };

    return transaction;
}
```
- example usage
```shell
...
var transaction = new EventEmitter();
transaction.isTransaction = true;
transaction.origin = schema;
transaction.name = schema.name;
transaction.settings = schema.settings;
transaction.connected = false;
transaction.connecting = false;
transaction.adapter = schema.adapter.transaction();

// create blank models pool
transaction.models = {};
transaction.definitions = {};

for (var i in schema.models) {
    schema.copyModel.call(transaction, schema.models[i]);
...
```



# <a name="apidoc.module.jugglingdb.Schema.types"></a>[module jugglingdb.Schema.types](#apidoc.module.jugglingdb.Schema.types)

#### <a name="apidoc.element.jugglingdb.Schema.types.JSON"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.types.</span>JSON ()](#apidoc.element.jugglingdb.Schema.types.JSON)
- description and source-code
```javascript
function JSON() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.Schema.types.Text"></a>[function <span class="apidocSignatureSpan">jugglingdb.Schema.types.</span>Text (s)](#apidoc.element.jugglingdb.Schema.types.Text)
- description and source-code
```javascript
function Text(s) { return s; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.jutil"></a>[module jugglingdb.jutil](#apidoc.module.jugglingdb.jutil)

#### <a name="apidoc.element.jugglingdb.jutil.inherits"></a>[function <span class="apidocSignatureSpan">jugglingdb.jutil.</span>inherits (newClass, baseClass)](#apidoc.element.jugglingdb.jutil.inherits)
- description and source-code
```javascript
inherits = function (newClass, baseClass) {
    Object.keys(baseClass).forEach(function (classMethod) {
        newClass[classMethod] = baseClass[classMethod];
    });
    Object.keys(baseClass.prototype).forEach(function (instanceMethod) {
        newClass.prototype[instanceMethod] = baseClass.prototype[instanceMethod];
    });
}
```
- example usage
```shell
...
                   }
               }
           });
       });
   };
}

util.inherits(Schema, EventEmitter);

/**
* Define class
*
* @param {String} className
* @param {Object} properties - hash of class properties in format
*   '{property: Type, property2: Type2, ...}'
...
```



# <a name="apidoc.module.jugglingdb.list"></a>[module jugglingdb.list](#apidoc.module.jugglingdb.list)

#### <a name="apidoc.element.jugglingdb.list.list"></a>[function <span class="apidocSignatureSpan">jugglingdb.</span>list (data, type, parent)](#apidoc.element.jugglingdb.list.list)
- description and source-code
```javascript
function List(data, type, parent) {
    var list = this;
    if (!(list instanceof List)) {
        return new List(data);
    }

    if (data && data instanceof List) data = data.items;

    Object.defineProperty(list, 'parent', {
        writable: false,
        enumerable: false,
        configurable: false,
        value: parent
    });

    Object.defineProperty(list, 'nextid', {
        writable: true,
        enumerable: false,
        value: 1
    });

    var Item = ListItem;
    if (typeof type === 'object' && type.constructor.name === 'Array') {
        Item = type[0] || ListItem;
    }

    data = list.items = data || [];
    Object.defineProperty(list, 'ItemType', {
        writable: true,
        enumerable: false,
        configurable: true,
        value: Item
    });

    if ('string' === typeof data) {
        try {
            list.items = data = JSON.parse(data);
        } catch(e) {
            list.items = data = [];
        }
    }

    data.forEach(function(item, i) {
        data[i] = new Item(item, list);
        Object.defineProperty(list, data[i].id, {
            writable: true,
            enumerable: false,
            configurable: true,
            value: data[i]
        });
        if (list.nextid <= data[i].id) {
            list.nextid = data[i].id + 1;
        }
    });

    Object.defineProperty(list, 'length', {
        enumerable: false,
        configurable: true,
        get: function() {
            return list.items.length;
        }
    });

    return list;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.list.prototype"></a>[module jugglingdb.list.prototype](#apidoc.module.jugglingdb.list.prototype)

#### <a name="apidoc.element.jugglingdb.list.prototype.autoincrement"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>autoincrement ()](#apidoc.element.jugglingdb.list.prototype.autoincrement)
- description and source-code
```javascript
autoincrement = function () {
    return this.nextid++;
}
```
- example usage
```shell
...
Object.defineProperty(this, 'parent', {
    writable: false,
    enumerable: false,
    configurable: true,
    value: parent
});
if (!this.id) {
    this.id = parent.autoincrement();
}
if (parent.ItemType) {
    this.__proto__ = parent.ItemType.prototype;
    if (parent.ItemType !== ListItem) {
        parent.ItemType.apply(this);
    }
}
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.concat"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>concat ()](#apidoc.element.jugglingdb.list.prototype.concat)
- description and source-code
```javascript
concat = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.every"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>every ()](#apidoc.element.jugglingdb.list.prototype.every)
- description and source-code
```javascript
every = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.filter"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>filter ()](#apidoc.element.jugglingdb.list.prototype.filter)
- description and source-code
```javascript
filter = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...

var req = {
    'where': {}
};

if (!keyVals[relation.keyFrom]) {
    objsByKeys[relation.keyFrom] = {};
    objs.filter(Boolean).forEach(function (obj) {
        if (!objsByKeys[relation.keyFrom][obj[relation.keyFrom]]) {
            objsByKeys[relation.keyFrom][obj[relation.keyFrom]] = [];
        }
        objsByKeys[relation.keyFrom][obj[relation.keyFrom]].push(obj);
    });
    keyVals[relation.keyFrom] = Object.keys(objsByKeys[relation.keyFrom]);
}
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.find"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>find (pattern, field)](#apidoc.element.jugglingdb.list.prototype.find)
- description and source-code
```javascript
find = function (pattern, field) {
    if (!field) {
        field = 'id';
    }
    var res;
    this.items.forEach(function(o) {
        if (o[field] == pattern) res = o;
    });
    return res;
}
```
- example usage
```shell
...
// get one latest post
Post.findOne({where: {published: true}, order: 'date DESC'}, cb);
// same as new Post({userId: user.id});
user.posts.build
// save as Post.create({userId: user.id}, cb);
user.posts.create(cb)
// find instance by id
User.find(1, cb)
// count instances
User.count([conditions, ]cb)
// destroy instance
user.destroy(cb);
// destroy all instances
User.destroyAll(cb);
// update a post (currently only on the mysql adapter)
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.forEach"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>forEach ()](#apidoc.element.jugglingdb.list.prototype.forEach)
- description and source-code
```javascript
forEach = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
exports.__defineGetter__('BaseSQL', function () {
return require(baseSQL);
});

exports.loadSchema = function(filename, settings, compound) {
var schema = [];
var definitions = require(filename);
Object.keys(definitions).forEach(function(k) {
    var conf = settings[k];
    if (!conf) {
        console.log('No config found for ' + k + ' schema, using in-memory schema');
        conf = {driver: 'memory'};
    }
    schema[k] = new Schema(conf.driver, conf);
    schema[k].on('define', function(m, name, prop, sett) {
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>indexOf ()](#apidoc.element.jugglingdb.list.prototype.indexOf)
- description and source-code
```javascript
indexOf = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...

/**
* Inclusion validator
*/
function validateInclusion(attr, conf, err) {
   if (nullCheck.call(this, attr, conf, err)) return;

   if (!~conf.in.indexOf(this[attr])) {
       err();
   }
}

/**
* Exclusion validator
*/
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.inspect"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>inspect ()](#apidoc.element.jugglingdb.list.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
    return util.inspect(this.items);
}
```
- example usage
```shell
...
    });

    return list;

}

List.prototype.inspect = function() {
    return util.inspect(this.items);
};

var _;
try {
    var underscore = 'underscore';
    _ = require(underscore);
} catch (e) {
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.join"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>join ()](#apidoc.element.jugglingdb.list.prototype.join)
- description and source-code
```javascript
join = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
    if (!config) {
        console.log('No environment ' + env + ' found in config/database.{js|json|yml}');
        throw new Error('No environment ' + env + ' found in config/database.{js|json|yml}');
    }

    // when driver name started with point - look for driver in app root (relative path)
    if (config.driver && config.driver.match(/^\./)) {
        config.driver = path.join(app.root, config.driver);
    }

    schema = new Schema(config && config.driver || 'memory', config);
    schema.log = log;
    if (!schema.adapter) throw new Error('Adapter is not defined');

} else {
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>lastIndexOf ()](#apidoc.element.jugglingdb.list.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.map"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>map (cb)](#apidoc.element.jugglingdb.list.prototype.map)
- description and source-code
```javascript
map = function (cb) {
    if (typeof cb === 'function') {
        return this.items.map(cb);
    }
    if (typeof cb === 'string') {
        return this.items.map(function(el) {
            if (typeof el[cb] === 'function') {
                return el[cb]();
            }
            if (el.hasOwnProperty(cb)) {
                return el[cb];
            }
        });
    }
}
```
- example usage
```shell
...
    delete this[id];
    this.items.splice(found, 1);
}
};

List.prototype.map = function(cb) {
if (typeof cb === 'function') {
    return this.items.map(cb);
}
if (typeof cb === 'string') {
    return this.items.map(function(el) {
        if (typeof el[cb] === 'function') {
            return el[cb]();
        }
        if (el.hasOwnProperty(cb)) {
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.pop"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>pop ()](#apidoc.element.jugglingdb.list.prototype.pop)
- description and source-code
```javascript
pop = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
        enumerable: false,
        value: []
    });
}
args = [].slice.call(args);
var conf;
if (typeof args[args.length - 1] === 'object') {
    conf = args.pop();
} else {
    conf = {};
}
if (validation === 'custom' && typeof args[args.length - 1] === 'function') {
    conf.customValidator = args.pop();
}
conf.validation = validation;
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.push"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>push (obj)](#apidoc.element.jugglingdb.list.prototype.push)
- description and source-code
```javascript
push = function (obj) {
    var item = new ListItem(obj, this);
    this.items.push(item);
    return item;
}
```
- example usage
```shell
...
schema[k].on('define', function(m, name, prop, sett) {
    compound.models[name] = m;
    if (conf.backyard) {
        schema[k].backyard.define(name, prop, sett);
    }
});
schema[k].name = k;
schema.push(schema[k]);
if (conf.backyard) {
    schema[k].backyard = new Schema(conf.backyard.driver, conf.backyard);
}
if ('function' === typeof definitions[k]) {
    define(schema[k], definitions[k]);
    if (conf.backyard) {
        define(schema[k].backyard, definitions[k]);
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.remove"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>remove (obj)](#apidoc.element.jugglingdb.list.prototype.remove)
- description and source-code
```javascript
remove = function (obj) {
    var id = obj.id ? obj.id : obj;
    var found = false;
    this.items.forEach(function(o, i) {
        if (id && o.id == id) {
            found = i;
            if (o.id !== id) {
                console.log('WARNING! Type of id not matched');
            }
        }
    });
    if (found !== false) {
        delete this[id];
        this.items.splice(found, 1);
    }
}
```
- example usage
```shell
...
// post.author() -- sync getter when called without params
// post.author(user) -- setter when called with object

User.hasAndBelongsToMany('groups');
// user.groups(callback) - get groups of user
// user.groups.create(data, callback) - create new group and connect with user
// user.groups.add(group, callback) - connect existing group with user
// user.groups.remove(group, callback) - remove connection between group and user

schema.automigrate(); // required only for mysql and postgres NOTE: it will drop User and Post tables

// work with models:
var user = new User;
user.save(function (err) {
var post = user.posts.build({title: 'Hello world'});
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.removeAt"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>removeAt (index)](#apidoc.element.jugglingdb.list.prototype.removeAt)
- description and source-code
```javascript
removeAt = function (index) {
    this.splice(index, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.reverse"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>reverse ()](#apidoc.element.jugglingdb.list.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.shift"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>shift ()](#apidoc.element.jugglingdb.list.prototype.shift)
- description and source-code
```javascript
shift = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
    function destroyAll(cb) {
targetClass.all(this._scope, function (err, data) {
    if (err) {
        cb(err);
    } else {
        (function loopOfDestruction (data) {
            if(data.length > 0) {
                data.shift().destroy(function(err) {
                    if(err && cb) cb(err);
                    loopOfDestruction(data);
                });
            } else {
                if(cb) cb();
            }
        }(data));
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.slice"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>slice ()](#apidoc.element.jugglingdb.list.prototype.slice)
- description and source-code
```javascript
slice = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
        } else if (done) {
            done.call(this);
        }
    }
};

function capitalize(string) {
    return string.charAt(0).toUpperCase() + string.slice(1);
}
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.some"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>some ()](#apidoc.element.jugglingdb.list.prototype.some)
- description and source-code
```javascript
some = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.sort"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>sort ()](#apidoc.element.jugglingdb.list.prototype.sort)
- description and source-code
```javascript
sort = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.splice"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>splice ()](#apidoc.element.jugglingdb.list.prototype.splice)
- description and source-code
```javascript
splice = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
    this.items.forEach(function(o) {
        if (o[field] == pattern) res = o;
    });
    return res;
};

List.prototype.removeAt = function(index) {
    this.splice(index, 1);
};

List.prototype.toObject = function() {
    return this.items;
};

List.prototype.toJSON = function() {
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toJSON ()](#apidoc.element.jugglingdb.list.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    return this.items;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.toObject"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toObject ()](#apidoc.element.jugglingdb.list.prototype.toObject)
- description and source-code
```javascript
toObject = function () {
    return this.items;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.toSource"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toSource ()](#apidoc.element.jugglingdb.list.prototype.toSource)
- description and source-code
```javascript
toSource = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jugglingdb.list.prototype.toString"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>toString ()](#apidoc.element.jugglingdb.list.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return JSON.stringify(this.items);
}
```
- example usage
```shell
...
} else if (existsSync(schemaFile + 'coffee')) {
    schemaFile += 'coffee';
} else {
    schemaFile = false;
}

if (schemaFile) {
    var code = fs.readFileSync(schemaFile).toString();
    if (schemaFile.match(/\.coffee$/)) {
        code = require('coffee-script').compile(code);
    }
    /*jshint evil: true */
    var fn = new Function('context', 'require', 'with(context){(function(){' + code + '})()}');
    fn(context, require);
}
...
```

#### <a name="apidoc.element.jugglingdb.list.prototype.unshift"></a>[function <span class="apidocSignatureSpan">jugglingdb.list.prototype.</span>unshift ()](#apidoc.element.jugglingdb.list.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
    return Array.prototype[method].apply(this.items, slice.call(arguments));
}
```
- example usage
```shell
...
        'lastIndexOf',
        'range'
    ];

    _import.forEach(function(name) {
        List.prototype[name] = function() {
            var args = [].slice.call(arguments);
            args.unshift(this.items);
            return _[name].apply(_, args);
        };
    });
}

// copy all array methods
[   'concat',
...
```



# <a name="apidoc.module.jugglingdb.schema"></a>[module jugglingdb.schema](#apidoc.module.jugglingdb.schema)

#### <a name="apidoc.element.jugglingdb.schema.Schema"></a>[function <span class="apidocSignatureSpan">jugglingdb.schema.</span>Schema (name, settings)](#apidoc.element.jugglingdb.schema.Schema)
- description and source-code
```javascript
function Schema(name, settings) {
    var schema = this;
    // just save everything we get
    this.name = name;
    this.settings = settings || {};

    // Disconnected by default
    this.connected = false;
    this.connecting = false;

    // create blank models pool
    this.models = {};
    this.definitions = {};

    if (this.settings.log) {
        this.on('log', function(str, duration) {
            console.log(str);
        });
    }

    // and initialize schema using adapter
    // this is only one initialization entry point of adapter
    // this module should define 'adapter' member of 'this' (schema)
    var adapter;
    if (typeof name === 'object') {
        adapter = name;
        this.name = adapter.name;
    } else if (name.match(/^\//)) {
        // try absolute path
        adapter = require(name);
    } else if (existsSync(__dirname + '/adapters/' + name + '.js')) {
        // try built-in adapter
        adapter = require('./adapters/' + name);
    } else {
        // try foreign adapter
        try {
            adapter = require('jugglingdb-' + name);
        } catch (e) {
            return console.log('\nWARNING: JugglingDB adapter "' + name + '" is not installed,\nso your models would not work, to
 fix run:\n\n    npm install jugglingdb-' + name, '\n');
        }
    }

    this.connecting = true;
    adapter.initialize(this, function () {

        this.adapter.log = function (query, start) {
            schema.log(query, start);
        };

        this.adapter.logger = function (query) {
            var t1 = Date.now();
            var log = this.log;
            return function (q) {
                log(q || query, t1);
            };
        };

        this.connecting = false;
        this.connected = true;
        this.emit('connected');

    }.bind(this));

    // we have an adaper now?
    if (!this.adapter) {
        this.emit('disconnected');
        throw new Error('Adapter "' + name + '" is not defined correctly: it should define 'adapter' member of schema synchronously
');
    }

    schema.connect = function(cb) {
        var schema = this;
        schema.connecting = true;
        return new when.Promise(function(resolve, reject) {
            if (!schema.adapter.connect) {
                return process.nextTick(function() {
                    schema.connecting = false;
                    if (cb) {
                        cb(null, schema);
                    }
                    return resolve(schema);
                });
            }
            schema.adapter.connect(function(err) {
                if (err) {
                    schema.connected = false;
                    schema.connecting = false;
                    reject(err);
                    if (cb) {
                        cb(err);
                    }
                } else {
                    schema.connected = true;
                    schema.connecting = false;
                    schema.emit('connected');
                    resolve(schema);
                    if (cb) {
                        cb(null, schema);
                    }
                }
            });
        });
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.scope"></a>[module jugglingdb.scope](#apidoc.module.jugglingdb.scope)

#### <a name="apidoc.element.jugglingdb.scope.defineScope"></a>[function <span class="apidocSignatureSpan">jugglingdb.scope.</span>defineScope (cls, targetClass, name, params, methods)](#apidoc.element.jugglingdb.scope.defineScope)
- description and source-code
```javascript
function defineScope(cls, targetClass, name, params, methods) {

    // collect meta info about scope
    if (!cls._scopeMeta) {
        cls._scopeMeta = {};
    }

    // only makes sence to add scope in meta if base and target classes
    // are same
    if (cls === targetClass) {
        cls._scopeMeta[name] = params;
    } else {
        if (!targetClass._scopeMeta) {
            targetClass._scopeMeta = {};
        }
    }

    Object.defineProperty(cls, name, {
        enumerable: false,
        configurable: true,
        get: function () {
            var f = function caller(condOrRefresh, cb) {
                var actualCond = {};
                var actualRefresh = false;
                var saveOnCache = true;
                if (arguments.length === 1) {
                    cb = condOrRefresh;
                } else if (arguments.length === 2) {
                    if (typeof condOrRefresh === 'boolean') {
                        actualRefresh = condOrRefresh;
                    } else {
                        actualCond = condOrRefresh;
                        actualRefresh = true;
                        saveOnCache = false;
                    }
                } else {
                    throw new Error('Method can be only called with one or two arguments');
                }

                if (!this.__cachedRelations || (typeof this.__cachedRelations[name] == 'undefined') || actualRefresh) {
                    var self = this;
                    var params = mergeParams(actualCond, caller._scope);
                    return targetClass.all(params, function(err, data) {
                        if (!err && saveOnCache) {
                            if (!self.__cachedRelations) {
                                self.__cachedRelations = {};
                            }
                            self.__cachedRelations[name] = data;
                        }
                        cb(err, data);
                    });
                } else {
                    cb(null, this.__cachedRelations[name]);
                }
            };
            f._scope = typeof params === 'function' ? params.call(this) : params;
            f.build = build;
            f.create = create;
            f.destroyAll = destroyAll;
            for (var i in methods) {
                f[i] = methods[i].bind(this);
            }

            // define sub-scopes
            Object.keys(targetClass._scopeMeta).forEach(function (name) {
                Object.defineProperty(f, name, {
                    enumerable: false,
                    get: function () {
                        mergeParams(f._scope, targetClass._scopeMeta[name]);
                        return f;
                    }
                });
            }.bind(this));
            return f;
        }
    });

    // and it should have create/build methods with binded thisModelNameId param
    function build(data) {
        return new targetClass(mergeParams(this._scope, {where:data || {}}).where);
    }

    function create(data, cb) {
        if (typeof data === 'function') {
            cb = data;
            data = {};
        }
        this.build(data).save(cb);
    }

<span class="apidocCodeCommentSpan">    /*
        Callback
        - The callback will be called after all elements are destroyed
        - For every destroy call which results in an error
        - If fetching the Elements on which destroyAll is called results in an error
    */
</span>    function destroyAll(cb) {
        targetClass.all(this._scope, function (err, data) {
            if (err) {
                cb(err);
            } else {
                (function loopOfDestruction (data) {
                    if(data.length > 0) {
                        data.shift().destroy(function(err) {
                            if(err && cb) cb(err);
                            loopOfDestruction(data);
                        });
                    } else {
                        if(cb) cb();
                    }
                }(data));
            }
        });
    }

    function mergeParams(base, update) {
        if (updat ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.utils"></a>[module jugglingdb.utils](#apidoc.module.jugglingdb.utils)

#### <a name="apidoc.element.jugglingdb.utils.safeRequire"></a>[function <span class="apidocSignatureSpan">jugglingdb.utils.</span>safeRequire (module)](#apidoc.element.jugglingdb.utils.safeRequire)
- description and source-code
```javascript
function safeRequire(module) {
    try {
        return require(module);
    } catch (e) {
        console.log('Run "npm install jugglingdb ' + module + '" command to use jugglingdb using ' + module + ' database engine');
        process.exit(1);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jugglingdb.validations"></a>[module jugglingdb.validations](#apidoc.module.jugglingdb.validations)

#### <a name="apidoc.element.jugglingdb.validations.ValidationError"></a>[function <span class="apidocSignatureSpan">jugglingdb.validations.</span>ValidationError (obj)](#apidoc.element.jugglingdb.validations.ValidationError)
- description and source-code
```javascript
function ValidationError(obj) {
    if (!(this instanceof ValidationError)) return new ValidationError(obj);

    this.name = 'ValidationError';
    this.message = 'Validation error';
    this.statusCode = 400;
    this.codes = obj.errors && obj.errors.__codes;
    this.context = obj && obj.constructor && obj.constructor.modelName;

    Error.call(this);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
