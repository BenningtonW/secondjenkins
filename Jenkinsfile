
pipeline {
    agent any

    stages {
        stage('gitget') {
            steps {
                git branch: 'main', url: 'https://github.com/BenningtonW/secondjenkins.git'
              
              
            }
          
               stage('runscript') {
            steps {
                sh 'myscript'
              
              
            }     
                   
                   stage('archive') {
            steps {
                archiveArtifacts artifacts: 'output', followSymlinks: false
              
              
            }
        }
    }
}






