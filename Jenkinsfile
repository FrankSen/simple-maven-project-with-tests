pipeline {
  agent any

  tools{
     maven "maven_3_5_0"
  }

  stages {

    stage('Compile Stage') {
        steps{
            sh 'mvn clean compile'
        }
    }

    stage('Test Stage'){
        steps{
            sh 'mvn test'
        }
    }

    stage('Deploy stage'){
        steps{
            sh 'mvn clean package'
        }
    }
  }
}