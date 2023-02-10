pipeline {
    agent any
    stages {
        stage('publish over ssh') {
            steps {
                sshPublisher(publishers: [sshPublisherDesc(configName: 'httpd server', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '**/*')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])

            }
        }
        
    }
}
