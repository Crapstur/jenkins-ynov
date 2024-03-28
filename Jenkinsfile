node {
    stage('Clone') {
        git branch: 'main',
            url: 'https://github.com/Crapstur/jenkins-ynov.git'
    }
    // stage('TMP') {
    //     sh 'whoami'
    // }
    stage('Docker') {
        sh 'docker build -t crapstur/roundcubemail .'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,
          playbook: 'playbook.yml'
      )
    }
}