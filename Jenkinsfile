node {
    stage('Pull RoundCube image') {
        sh 'docker pull roundcube/roundcubemail:latest'
    }
    stage('Deploy RoundCube') {
        sh 'docker run -d -p 8081:80 roundcube/roundcubemail:latest'
    }
}