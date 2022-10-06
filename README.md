## Disclaimer ##
This is a fork of [orginial SlowHTTPTest](https://github.com/shekyan/slowhttptest). Modified by RxnNode to suit the needs.

Any actions and or activities related to the code provided is solely your responsibility.The misuse of the information in this website can result in criminal charges brought against the persons in question. The authors will not be held responsible in the event any criminal charges be brought against any individuals misusing the information in this tool to break the law.


# SlowHTTPTest #

[![Build Status](https://travis-ci.org/shekyan/slowhttptest.svg?branch=master)](https://travis-ci.org/shekyan/slowhttptest)

SlowHTTPTest is a highly configurable tool that simulates some Application Layer Denial of Service attacks by prolonging HTTP connections in different ways.

Use it to test your web server for DoS vulnerabilites, or just to figure out how many concurrent connections it can handle.
SlowHTTPTest works on majority of Linux platforms, OS X and Cygwin - a Unix-like environment and command-line interface for Microsoft Windows, and comes with a Dockerfile to make things even easier.

Check out [Wiki](https://github.com/shekyan/slowhttptest/wiki) for installation and usage details.

Latest official image is available at [Docker Hub](https://hub.docker.com/repository/docker/shekyan/slowhttptest):
`docker pull shekyan/slowhttptest:latest`

# Modified #

+ update user-agent and remove signatures
+ **Listed Query** mode
    Supply a file that contains a line-separated list of values. If upplied, a value will be picked randomly from the list, then t forms a key-value pair, 'q=<value>', which is appended to the end of url.