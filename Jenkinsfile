node {
    checkout scm

    docker.withRegistry('', 'DockerHub') {
        def dockerfile = 'Dockerfile'
        def customImage = docker.build("umateakshay/pizzaluvrs:${env.BUILD_ID}", "-f ${dockerfile} ./")
       /* def customImage = docker.build("pizzaLuvrs:${env.BUILD_ID}") */
        /*def customImage1 = docker.build("umateakshay/test:${env.BUILD_ID}")*/
        /*def customImage1 = 'umateakshay/test'*/
        /* Push the container to the custom Registry */
        customImage.push()
    }
}
