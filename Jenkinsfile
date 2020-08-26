node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/repository/docker', 'DockerHub') {

        def customImage = docker.build("PizzaLuvrs:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
