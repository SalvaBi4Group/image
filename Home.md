# Guide to developing using draw.io

draw.io consists of two parts, currently. The main part is the client-side JavaScript code. You can create the minified JavaScript using the default "all" task of the [Ant build.xml file](https://github.com/jgraph/draw.io/blob/master/etc/build/build.xml). After building the minified JavaScript, point a web server at the /war directory and you'll get the client functionality served at /index.html.

One easy way to deploy is to map the Github pages site to your master branch, [as we have done on the master project](https://jgraph.github.io/draw.io/war/index.html).

To build the Java server-side code into a war invokes the "war" task in the [Ant build.xml file](https://github.com/jgraph/draw.io/blob/master/etc/build/build.xml). Deploy the resulting .war file to a servlet engine.

The server-side functionality currently consists of Gliffy import, .vsdx import, Iconfinder search and publish to Imgur.

[[Translations|translations]]