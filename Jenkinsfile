pipeline {
    agent any
    stages {
        stage('Dev Server Configuration') {
  
    steps {
       sshPublisher(publishers: [sshPublisherDesc(configName: 'Ansible-Control-Machine', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: 'ansible-playbook -i /home/ubuntu/live-project/dev.inventory /home/ubuntu/live-project/site.yml', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/home/ubuntu/live-project/', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
    }
  }
    }
}
