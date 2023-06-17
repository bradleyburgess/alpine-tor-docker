# tor-docker

This is a fork of [andrius/alpine-tor](https://github.com/andrius/alpine-tor).

I forked this with the intention of using it as a command line tor client in
conjunction with `lynx` and `curl`, to run on a headless / TTY server.

First, start the container with `docker run -d --name tor-docker 
bradleyburgess/tor-docker`. Then you can pass whatever commands you want via 
`docker exec`, using the `torify` wrapper; e.g. 
`docker exec -it tor-docker torify lynx https://check.torproject.org`.

You can obviously use bash / zsh aliases to make this easier.
