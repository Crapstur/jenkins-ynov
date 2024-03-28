node {
    stage('Clone') {
        git branch: 'main',
            url: 'https://github.com/Crapstur/jenkins-ynov.git'
    }
    stage('Docker Build') {
        sh 'cd jenkins-ynov && docker build -t jenkins-ynov .'
    }
    // stage('Ansible') {
    //   ansiblePlaybook (
    //       colorized: true, 
    //       become: true,
    //       playbook: 'playbooks/deploy-app.yaml',
    //       inventory: 'hosts/hosts.ini'
    //   )
    // }
}