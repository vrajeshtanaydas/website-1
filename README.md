website
=======

GeoNetwork opensource website project. The content of this repository is 
deployed as a website at http://geonetwork-opensource.org

Website build
=============

Required software:
 
* git, 
* sphinx, 
* make (Linux, OSX or a unix emulator on Windows) or maven

First checkout the website source:

```
  git clone -b master https://github.com/geonetwork/website.git .
```


Retrieve user and developer docs using shell script:

```
  ./checkup_docs.sh
```

Run make html in docsrc to build website using sphinx:

```
  make html
```

or maven
```
  mvn clean install
```


Copy the javadoc to the build/html folder:
  
```
  cp -fr ../../trunk/docs/build/html/javadoc build/html/.
```

Publish the website on http://geonetwork-opensource.org
