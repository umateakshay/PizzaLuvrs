node {
    checkout scm

    docker.withRegistry('', 'DockerHub') {
        def dockerfile = 'Dockerfile'
        def customImage = docker.build("pizzaluvrs:${env.BUILD_ID}", "-f ${dockerfile} ./")
       /* def customImage = docker.build("pizzaLuvrs:${env.BUILD_ID}") */

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
