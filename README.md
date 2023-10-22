Docker DNS-O-Matic for Raspberry Pi
==================

> 📘 This is a fork from [codeworksio/docker-dnsomatic' original repo](https://github.com/codeworksio/docker-dnsomatic).

Easily announce your new IP address to the world.

Installation
------------

Builds of the image are available on [Docker Hub](https://hub.docker.com/r/antoineraulin/dnsomatic-rpi/) where you can download from the latest stable image.

    docker pull araulin/dnsomatic-rpi

Alternatively you can build the image yourself.

    docker build --tag araulin/dnsomatic-rpi \
        github.com/antoineraulin/docker-dnsomatic-rpi

Quickstart
----------

Start container using:

    docker run --detach --restart always \
        --name dnsomatic \
        --hostname dnsomatic \
        --env "DNSOMATIC_USERNAME=username" \
        --env "DNSOMATIC_PASSWORD=password" \
        --env "TZ=timezone" \
        araulin/dnsomatic-rpi

See
---

* [DNS-O-Matic API](https://www.dnsomatic.com/wiki/api)
* [List of valid timezones](https://gist.github.com/heyalexej/8bf688fd67d7199be4a1682b3eec7568)
