[![Build Status](https://travis-ci.org/codetojoy/easter_eggs_for_java_9.svg?branch=master)](https://travis-ci.org/codetojoy/easter_eggs_for_java_9)

### Eggs for Java 9 Modules

* some basic examples for Java 9 modules 
* usage of *'egg'* here is [SSCCE](http://sscce.org/) **not** a [hidden feature](https://en.wikipedia.org/wiki/Easter_egg_(media)) !
* see notes below to use JDK9 in Docker
* see README.md in each folder for steps to execute

### validation log
* confirmed 12-MAY-2017 with b169 via Docker automenta/javai [image](https://hub.docker.com/r/automenta/javai/)
    * set JAVA_HOME for jlink
* confirmed 05-MAY-2017 with b168 via Docker automenta/javai [image](https://hub.docker.com/r/automenta/javai/)
    * set JAVA_HOME for jlink
* confirmed 05-MAY-2017 with b167 via sdkman
* confirmed 03-APR-2017 with b161

### Setup for Docker

* These instructions work for Mac OS X. Tweak as appropriate
* Install Docker from [here](https://www.docker.com/) 
* Open 'Docker Quick Start Terminal'

* set `MY_SRC_HOME` to be appropriate directory on your computer where this repo is located
* execute the following (one command at a time):

<pre>
docker pull automenta/javai:latest
cd $MY_SRC_HOME
docker run --rm -t -i -v $(pwd):/data automenta/javai bash
export JAVA_HOME=/j/jdk9/bin
cd /data
</pre>
