# Compojure-Template

A Leiningen template for web app projects using Compojure, Hiccup and Bootstrap. 

This tempate is based on [compojure-template](https://github.com/yogthos/compojure-template). 

## Usage

Run the following command to create a new Compojure project:

    lein new webapp <your project name>

To create a standalone executable from your project inside the project directory:

```bash
lein ring uberjar
```

You can then run the resulting jar as you would with any other Java executable:

```bash
java -jar target/myapp-0.1.0-SNAPSHOT-standalone.jar

2012-12-15 19:17:23.471:INFO:oejs.Server:jetty-7.x.y-SNAPSHOT
2012-12-15 19:17:23.512:INFO:oejs.AbstractConnector:Started SelectChannelConnector@0.0.0.0:8080
Server started on port [ 8080 ].
You can view the site at http://localhost:8080
```

To build a WAR run:
```bash
lein ring uberwar
```
Then you can deploy the resulting WAR to Tomcat or any other Java application server.

## License

Copyright © 2012 Anthony Manoras

Distributed under the Eclipse Public License, the same as Clojure.
