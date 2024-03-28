node {
    stage('Clone') {
        git branch: 'main',
            url: 'https://github.com/Crapstur/jenkins-ynov.git'
    }
    stage('TMP') {
        sh 'ls -l'
    }
    // stage('Docker Build') {
    //     sh 'docker build -t jenkins-ynov .'
    // }
    // stage('Ansible') {
    //   ansiblePlaybook (
    //       colorized: true, 
    //       become: true,
    //       playbook: 'playbooks/deploy-app.yaml',
    //       inventory: 'hosts/hosts.ini'
    //   )
    // }
}