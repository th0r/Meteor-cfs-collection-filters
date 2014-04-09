## Public and Private API ##

_API documentation automatically generated by [docmeteor](https://github.com/raix/docmeteor)._

***

__File: ["filters.js"](filters.js) Where: {client|server}__

***

### <a name="FS.Collection.prototype.filters"></a>*fsCollection*.filters(filters)&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ###

*This method __filters__ is defined in `prototype` of `FS.Collection`*

__Arguments__

* __filters__ *{Object}*  

 File filters for this collection.


__Returns__  *{undefined}*


> ```FS.Collection.prototype.filters = function fsColFilters(filters) { ...``` [filters.js:7](filters.js#L7)


-

### <a name="FS.Collection.prototype.allowsFile"></a>*fsCollection*.allowsFile()&nbsp;&nbsp;<sub><i>Anywhere</i></sub> ###

*This method __allowsFile__ is defined in `prototype` of `FS.Collection`*

__Returns__  *{boolean}*
True if the collection allows this file.


Checks based on any filters defined on the collection. If the
file is not valid according to the filters, this method returns false
and also calls the filter `onInvalid` method defined for the
collection, passing it an English error string that explains why it
failed.

> ```FS.Collection.prototype.allowsFile = function fsColAllowsFile(fileObj) { ...``` [filters.js:107](filters.js#L107)


-

### <a name="contentTypeInList"></a>contentTypeInList(list, contentType)&nbsp;&nbsp;<sub><i>undefined</i></sub> ###

*This method is private*

__Arguments__

* __list__ *{[String[]](#String[])}*  

 Array of content types

* __contentType__ *{String}*  

 The content type


__Returns__  *{Boolean}*


Returns true if the content type is in the list, or if it matches
one of the special types in the list, e.g., "image/*".

> ```function contentTypeInList(list, contentType) { ...``` [filters.js:168](filters.js#L168)

