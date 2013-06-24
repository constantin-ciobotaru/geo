geo
===

Java utility methods for creating and performing calculations with geohashes.

Status: **pre-alpha**

Features
----------

* encodes geohashes from latitude, longitude to arbitrary length (`GeoHash.encodeHash()`)
* decodes latitude, longitude from geohashes (`GeoHash.decodeHash()`)
* finds adjacent hash in any direction (`GeoHash.adjacentHash()`)
* finds all 8 adjacent hashes to a hash (`GeoHash.neighbours()`)
* calculates hash length to enclose a bounding box (`GeoHash.hashLengthToEncloseBoundingBox`)
* calculates geohashes of given length to cover a bounding box. Returns coverage ratio as well (`GeoHash.coverBoundingBoxWithHashLength`)
* simple [api](https://xuml-tools.ci.cloudbees.com/job/geo%20site/site/apidocs/index.html)
* good performance (~3 million `GeoHash.encodeHash` calls per second on an I7, single thread)
* no mutable types exposed by api
* threadsafe 
* 100% [unit test coverage](https://xuml-tools.ci.cloudbees.com/job/geo%20site/site/cobertura/index.html) (for what that's worth of course!)
* Apache 2.0 licence

Primary source was a translation to java of https://github.com/davetroy/geohash-js/blob/master/geohash.js.

Continuous integration with Jenkins for this project is [here](https://xuml-tools.ci.cloudbees.com/). <a href="https://xuml-tools.ci.cloudbees.com/"><img  src="http://web-static-cloudfront.s3.amazonaws.com/images/badges/BuiltOnDEV.png"/></a>
 
Project reports including Javadocs are [here](https://xuml-tools.ci.cloudbees.com/job/geo%20site/site/project-reports.html).

