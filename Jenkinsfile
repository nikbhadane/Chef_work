node{
      stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '${sha1}']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '12345', refspec: '+refs/pull/*:refs/remotes/origin/pr/*', url: 'https://github.com/nikbhadane/Chef_work']]])
        }
      
      stage('Build code'){
        echo 'Hello World Indianss'
        sh 'ls -al'
        sh 'df -h'
        sh 'cat /etc/passwd'
        sh 'cat README.md'
        sh 'sleep 45'
        }
	  stage('Test Code'){
	    sh 'echo "This goal is to verify stagesss"'
	    sh 'sleep 10'
        sh 'cat /etc/passwd'
	   }
     }
