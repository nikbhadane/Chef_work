node {
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '**']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '12345', name: 'origin', refspec: '+refs/pull/*:refs/remotes/origin/pr/*', url: 'https://github.com/nikbhadane/Chef_work']]])
    }
    stage('Pending'){
        gitHubPRStatus githubPRMessage('${GITHUB_PR_COND_REF} run started')
    }
    stage('Build'){
        echo 'Hello World'
        sh 'ls -al'
        sh 'df -h'
        sh 'cat /etc/passwd'
    }
}
