# HAProxy with stdout log

This is a custom HAProxy Docker image built on top of haproxy:1.8.13-alpine. It's added socat as a facility to carry log from `/dev/log` socket to stdout.

To use this logging facility, please add `log /dev/log local0 <log level>` to your haproxy.cfg

Other configuration, please refer to official HAProxy Docker image at http://hub.docker.com/_/haproxy
