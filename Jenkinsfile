pipeline {
    agent any

    stages {
        stage('Deploy html site') {
            steps {
                sshPublisher(publishers: [sshPublisherDesc(configName: 'html_page', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/var/www/html/', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '**/*.html')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
            }
        }
    }
}
