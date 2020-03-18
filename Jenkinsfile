pipeline {
   agent any
   stages {
        stage ('checkout'){
            steps {
                git branch: 'master', url: 'https://github.com/sivaramap/no-inet-gke-cluster.git'
            }
        }
      stage('Build') {
        steps {
           sh './deploy.sh'
        }
     }
   }
}
