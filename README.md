
This fork adds a dump of design_doc/couchdb_odata.json no longer available below (found on wayback machine.) Also, see https://github.com/kangu/couchdb_odata for an updated readme.

Not sure if this still works, but intent is to use Tableau Public with CouchDB.

## Original Readme text:

A show and a list to serve your data from couchdb as an OData feed.  
  
==HowTo==    

I've uploaded a complete design document to cloudant at http://nisbus.cloudant.com/odata/_design/odata/  
Copy that to your db, add views if you like to filter your data.  
Your OData service will now live here:  

 [http://localhost:5984/yourdb/_design/odata/_show/odata_service/_design/odata](http://localhost:5984/yourdb/_design/odata/_show/odata_service/_design/odata)  

You can now point anything that is able to consume odata feeds to this location (ex. powerpivot for Excel) and browse through your couchdb data.  




