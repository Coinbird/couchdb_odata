
This fork adds a dump of [design doc](design_doc/couchdb_odata.json) no longer available below (found on wayback machine.) Also, see https://github.com/kangu/couchdb_odata for an updated readme.

Be sure to paste the design doc directly from the source. Pasting from Raw github view seems to strip the `"` characters.

Even though this was a really old repo, I was able to view the ddoc correctly in CouchDB 2.3.1.
http://localhost:5984/YOUR-DB-HERE/_design/odata/_show/odata_service/_design/odata

My intent was to use Tableau Public with this CouchDB OData data source. 
* I pass the above URL format, I get "Bad OData format. Make sure you are using a URL that points to a valid OData Source."
* But, passing http://localhost:5984/YOUR-DB-HERE/_design/odata/_list/odata_convert/everything appears to work, at least at a superficial level, although I don't seem to get all my data in Tableau

* It would be cool to update this to return OData JSON format, instead of XML.
https://www.odata.org/documentation/


## Original Readme text:

A show and a list to serve your data from couchdb as an OData feed.  
  
==HowTo==    

I've uploaded a complete design document to cloudant at http://nisbus.cloudant.com/odata/_design/odata/  
Copy that to your db, add views if you like to filter your data.  
Your OData service will now live here:  

 [http://localhost:5984/yourdb/_design/odata/_show/odata_service/_design/odata](http://localhost:5984/yourdb/_design/odata/_show/odata_service/_design/odata)  

You can now point anything that is able to consume odata feeds to this location (ex. powerpivot for Excel) and browse through your couchdb data.  




