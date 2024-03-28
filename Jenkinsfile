// node {
//     stage('Pull RoundCube image') {
//         sh 'docker pull roundcube/roundcubemail:latest'
//     }
//     stage('Deploy RoundCube') {
//         sh 'docker run -d -p 8081:80 roundcube/roundcubemail:latest'
//     }
// }

node {
    stage('Git Clone') {
        git branch: 'main',
            url: 'https://github.com/Crapstur/jenkins-ynov.git'
    }
    stage('Docker Build') {
        sh 'docker build -t crapstur/roundcubemail .'
    }
    stage('Docker Run') {
        sh 'docker run -d -p 80:80 crapstur/roundcube'
    }
}