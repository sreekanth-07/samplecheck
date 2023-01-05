pipeline {
  agent any
      stages {
        stage('git-clone') {
            steps {
            //git branch: 'main', credentialsId: 'git-token', url: 'https://github.com/rajsekha/logs-store.git'
              bat'''
               git config --global user.email "Rajsekhar9912@gmail.com"
               git config --global user.name "rajsekha"
               git config --global user.password "Happy@1818'
               '''
             }
        }
       stage("git-push") {
            steps {
	          bat'''
	           git branch -a
	           git status
	           git add ouputlogs
               git commit -m "update changes"
               git push -u origin main
	           '''
	       }
        }
}

