node {
    checkout scm

    docker.withRegistry('', 'DockerHub') {

        def customImage = docker.build("pizzaLuvrs:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
