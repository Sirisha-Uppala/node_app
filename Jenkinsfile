node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/repository/docker/siri9911/nodeapp', 'dockerHub') {

        def customImage = docker.build("sirisha/nodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
