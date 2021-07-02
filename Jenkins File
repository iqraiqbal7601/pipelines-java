pipeline {
    agent any

 

    stages {
        stage('working directory clean') {
            steps {
                cleanWs()
            }
            }
     
        stage('git checkout'){
            steps {
                    git 'https://github.com/iqraiqbal7601/iqra-iqbal.git'
            }
        }
        
        stage('zipfile') {
            steps {
                zip dir: '', exclude: '', glob: '', zipFile: 'HRIS_TDDs'

 

            }
        }
            stage('Post Job') {  
                steps {
                 echo 'This will run only if successful'  
         }  
     } 
     post {
     always {
     //
}
success {
}
}

 }

 
