# Docker for rtc-switchboard

Docker image for [rtc-switchboard](https://github.com/rtc-io/rtc-switchboard), 
which is an rtc.io signalling server (counterpart to
[rtc-signaller](https://github.com/rtc-io/rtc-signaller)) that makes use of
the excellent realtime abstraction library,
[primus](https://github.com/primus/primus). It has been designed and built
primarily as a _reference implementation_ for a signalling server and is
not designed to be deployed at scale.

For more information about rtc-switchboard please visit: https://github.com/rtc-io/rtc-switchboard

You can find the docker builds here: https://registry.hub.docker.com/u/synctree/rtc-switchboard/

## Try it out

## Usage:

If you wish to use `rtc-switchboard` through a docker container
then you can simply pull the public image from hub.docker.io and 
run in the following way:

```
docker run synctree/rtc-switchboard
```

Defaults to 8080. If you wish to run the server on a specific port, then set the `NODE_PORT`
environment variable prior to execution:

```
docker run -e NODE_PORT=8997 synctree/rtc-switchboard
```

## Build your own image:

If you wish to build your own image using docker-rtc-switchboard:

```
docker build .
```


## License(s)

### Apache 2.0

Copyright 2014 Synctree, Inc.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
