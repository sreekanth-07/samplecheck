pipeline {
  agent any
      stages {
//         stage('git-clone') {
//             steps {
//             git branch: 'main', credentialsId: 'git-token', url: 'https://github.com/rajsekha/logs-store.git'
//               bat'''
//                git config --global user.email "kallepusreekanth7@gmail.com"
//                git config --global user.name "sreekanth-07"
//                git config --global user.password "K.sreekanth@1012'
//                '''
//              }
//         }
       stage("git-push") {
            steps {
	         bat'''
		    cd C:\\Users\\002XJB744\\Documents\\check
		    
	            git branch -a
	            git status
	            git add .
                    git status
                    git commit -m "update changes"
		    git pull
                    git push origin master
	            '''
	       }
        }
  }
}
