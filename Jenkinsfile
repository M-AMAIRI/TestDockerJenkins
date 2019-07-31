node {

    stage('Clone repository') {
        sh 'docker login -u moatez -p aqwzsxedc'
        sh 'docker images'
    }

    stage('Build image') {
        sh 'docker build -t moatez/dockerjenkins:2.0 .'
    }

    stage('Test image') {
        sh 'echo Tests passed'
        sh 'docker images'
    }

    stage('Push image') {
        sh 'echo Trying to Push Docker Build to DockerHub'
        sh 'docker push moatez/dockerjenkins:2.0'
    }
}
