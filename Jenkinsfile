node {
    stage('Clone') {
        git branch: 'main',
            url: 'https://github.com/Crapstur/jenkins-ynov.git'
    }
    stage('Docker') {
        sh 'docker build -t crapstur/roundcubemail .'
    }
    stage('Ansible') {
        sh 'ansible-playbook playbook.yml'
    }
    // stage('Ansible') {
    //   ansiblePlaybook (
    //       colorized: true,
    //       playbook: 'playbook.yml'
    //   )
    // }
}