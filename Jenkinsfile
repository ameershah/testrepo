node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerid') {

        def customImage = docker.build("ameershah/hwapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
