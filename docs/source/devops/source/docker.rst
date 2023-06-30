============
Docker
============

Get a list of containers and images

.. code:: bash

    # List all running containers
    docker ps

    # List all containers, including exited
    docker ps -a

    # Format the output to only show Image and Container Name
    docker ps --format "{{.Image}} - {{.Names}}"

    # List images
    docker images

----

Run and interact with containers

.. code:: bash

    # Run a container and remove it, when its finished
    docker run --rm <image>

    # Run a container and interact with it
    docker run -it --rm --name <container-name> <image> <command>

    # Interact with an already running container
    docker exec -it <container-name> <command>

----

Pull, build and push images

.. code:: bash

    # Download an image from a registry (e.g. python:3)
    docker pull <NAME[:TAG]>

    # Build image from Dockerfile locally
    docker build <path to Dockerfile>

    # Build image from Dockerfile with a name and tag
    docker build -t <username/repository-name:tag> <path to Dockerfile>

    # Publish image to docker registry
    docker push <username/repository-name:tag>

.. note:: 
    When pulling an image and no tag is provided, Docker uses the ``:latest`` tag as a default

.. note:: 
    If Dockerfile is located at the path of execution and is named ``Dockerfile`` the ``<path to Dockerfile>`` can be just a ``.``

----

Remove resources

.. code:: bash

    # Stop one or more running containers
    docker stop <name>

    # Remove one or more images
    docker image rm <name>

    # Remove unused images.
    docker image prune [-a]

    # Remove all stopped containers
    docker container prune

.. note:: 
    If ``-a`` is specified for ``image prune``, it will also remove all images not referenced by any container.
