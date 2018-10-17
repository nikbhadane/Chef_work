node {
    stage('Checkout'){
        checkout scm
    }
    stage('Pending'){
        gitHubPRStatus githubPRMessage('${GITHUB_PR_COND_REF} run started')
    }
    stage('Build'){
        echo 'Hello World'
        sh 'ls -al'
        sh 'df -h'
        sh 'cat /etc/passwd'
        sh 'cat README.md'
        sh 'cat \'Mastermind filesss\''
    }
}
