node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub-cred') {

        def customImage = docker.build("sirisha/nodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}