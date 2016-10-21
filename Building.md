# Building draw.io

draw.io consists of two parts, currently. The main part is the client-side JavaScript code. You can create the minified JavaScript using the default "all" task of the [Ant build.xml file](https://github.com/jgraph/draw.io/blob/master/etc/build/build.xml) which you can execute by running [`ant`](https://ant.apache.org/) in the `etc/build` folder of the repo. 

After building the minified JavaScript, point a web server at the /war directory and you'll get the client functionality served at /index.html.

One easy way to deploy is to map the Github pages site to your master branch, [as we have done on the master project](https://jgraph.github.io/draw.io/war/index.html).

Note, if you use just the client-side code, you'll be missing the Gliffy and .vsdx importers, the embed support ,icon search and publishing to Imgur.

If you want to build the full war with the Java server-side code and the client-side JavaScript, invoke the "war" task in the [Ant build.xml file](https://github.com/jgraph/draw.io/blob/master/etc/build/build.xml). Deploy the resulting .war file to a servlet engine.