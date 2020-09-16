node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("jenkins/jenkins")

        /* Push the container to the custom Registry */
       customImage.push('dockerkubernetes1992/nodeimage:nodejsimage')
    }
}
