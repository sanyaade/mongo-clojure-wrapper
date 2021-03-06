mongo-clojure-wrapper
=====================
mongo-clojure-wrapper is a wrapper around the official Mongo DB driver (mongo-java-driver). Only a subset has been implemented; development is ongoing. 

Sample Code
---------------

    (def db (struct db-config "TEST_DB" "localhost" 27017))
    (def collection "test_collection")

    (save-doc db collection {:name "Gilbert" :title "Mr"})
    (find-docs db collection {:name "Gilbert"})
    (delete-docs db collection {:title "Mr"})`

For more details, check the source code or the tests.

Usage
----------
Add mongo-clojure-wrapper.jar to your classpath and include the namespace 'mongodb.driver.

OR

Use leiningen and add '[mongo-clojure-wrapper "0.1.0"]' to your project.clj.

Links
---------
* [MongoDB](http://www.mongodb.com)
* [mongo-java-driver](http://www.mongodb.org/display/DOCS/Java+Language+Center)

