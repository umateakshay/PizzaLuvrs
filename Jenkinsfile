node {
    checkout scm

    docker.withRegistry('umateakshay/test', 'DockerHub') {

        def customImage = docker.build("PizzaLuvrs:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
