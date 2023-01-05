pipeline {
  agent any
  stages {
    stage('git-clone') {
//       steps {
//          bat '''
//          git clone https://github.com/sreekanth-07/samplecheck.git
//          '''
//           }
     }
      stage('git-push') {
            steps {
	          bat'''
                    cd C:\\Users\\002XJB744\\Documents\\check
                    ls
                    git init
	            git branch -a
	            git status
	            git add .
                    git status
                    git commit -m "update changes"
                    git push -u origin master
	          '''
	       }
        }
    
  }
}
