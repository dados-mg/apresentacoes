  "name": "A short url-usable (and preferably human-readable) name of the package. This MUST be lower-case and contain only alphanumeric characters along with “.”, “_” or “-” characters. It will function as a unique identifier and therefore SHOULD be unique in relation to any registry in which this package will be deposited (and preferably globally unique)",
  "title": "A string providing a title or one sentence description for this package",
  "profile": "Different kinds of data need different data and metadata formats. To support these different data and metadata formats we need to extend and specialise the generic Data Package. These specialized types of Data Package (or Data Resource) are termed profiles. For example, there is a Tabular Data Package profile that specializes Data Packages specifically for tabular data",
  "description": "A description of the package. The description MUST be markdown formatted",
  "homepage": "A URL for the home on the web that is related to this data package",
  "version": "A version string identifying the version of the package. It should conform to the Semantic Versioning requirements and should follow the Data Package Version pattern",
  "author":"name for person, name/title of organization",
  "license": "The license(s) under which the package is provided.",
  "keywords": "An Array of string keywords to assist users searching for the package in catalogs",
  "path": "property describing the location of the data associated to the resource, located online or locally on disk",
  "format": "‘csv’, ‘xls’, ‘json’ etc. Would be expected to be the standard file extension for this type of resource",  
  "encoding": "specify the character encoding of the resource’s data file. If no value for this key is specified then the default is UTF-8",
  "type":"string, number, integer, boolean, object, array, date, time, datetime, geopoint, geojson, etc",
  "format":"default, email, uri, any (depending of the type)"
