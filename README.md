Display JSON in Table with AngularJS
=================

Code licensed under MIT license.

This directive allow show your data in tables. It support searching, filtering and pagination.
Hight perfomance. Sorting feature is in progress...


## Installing via Bower
```
bower install angular-object-table
```

## Using

```
<link rel="stylesheet" type="text/css" href="{path to library}/build/object-table-style.css">

<script type="text/javascript" src="{path to library}/build/object-table.js"></script>

<!-- optional -->
<link rel="stylesheet" type="text/css" href="http://getbootstrap.com/dist/css/bootstrap.min.css">
```

Add HTML-markup :
```
<table object-table 
       from-url="http://some-url.com/getData" 
       data="exportDataVariable" 
       display="2" 
       headers="Name, Age" 
       fields="name, age"
></table>
```

## Atributes

Here is a file list for possible attributes for stable version:

Atribute             | Description
---------------------|----------------
data                 | - data source (array of objects)
fromUrl				 | - load data from external URL. Atribute 'data' or 'fromUrl' should be present
display     		 | *default: 5* - Display count. Using with pagging is displayed items per page
search               | *default: true* - Display search input 
pagging				 | *default: true* - Use pagging to present data
headers              | *required* - Example: ['HeaderName1','HeaderName2']. - Array of table header names
fields  			 | *optional* Example: ['property1','property2'].  - Array of displayed properties of object. This option allows you to display only certain fields of the object. Number of fields must be equal number of headers
