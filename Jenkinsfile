pipeline {
  agent any
//   parameters {
//     string(name: 'BRANCH', defaultValue: 'main', description: 'Namespace name', trim: true)
//   }
  stages {
    stage('PMD Scan') {
      steps {
        script {
          echo 'test'
//            bat '''  
//            cd bin
//            pmd -d ../src/main -R ../rulesetspmd.xml -f csv -r ../a.csv --fail-on-violation false
//            '''
        }
      }
    }
stage("git-push") {
               steps {
	       		
                     bat '''
		     
		     git config --global user.email "kallepusreekanth7@gmail.com"
                     git config --global user.name "sreekanth-07"
		     git config --global user.password "K.sreekanth@0585"
		     git branch -a
		     git checkout test
	             git status
	             git add .
                     git commit -m "update changes"
		     
		     git push https://github.com/sreekanth-07/samplecheck.git test
		     
	           '''
		   
		 }
           }
  }
}
