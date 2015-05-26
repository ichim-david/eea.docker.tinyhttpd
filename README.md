## Generic Docker image for Apache HTTP server based on Alpine Linux

This image is generic, thus you can obviously re-use it within your non-related EEA projects.

The difference from eeacms/httpd is that this image is derived from Alphine Linux
which gives you apache2 in an 9mb images instead of 325mb which is taken mostly by Centos 6.

### Tags
 - latest
 - alpine:3.1

### How to use this image
        $ docker run -it --rm -p 80:80 eeacms/tinyhttpd
        
### Server configuration
Build a Dockerfile with something similar:

        FROM eeacms/tinyhttpd
        
        ADD your-file.conf /etc/httpd/conf/httpd.conf
