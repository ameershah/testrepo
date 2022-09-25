node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerHubID') {

        def customImage = docker.build("ameer/helloworld")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
