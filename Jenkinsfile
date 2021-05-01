pipeline {
    agent { docker { image 'maven:3.3.3' } }
    parameters {
      string(name: 'INSTANCE_NAME',   defaultValue: 'YYY-QA-XXX',     description: 'Please enter your machine name like OAAA')
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'   
            }
        }
        
        stage('deploy') {
            steps {
                sh 'echo $INSTANCE_NAME'   
            }
        }
    }
}
