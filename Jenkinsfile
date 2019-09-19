@Library('jlibrary@main')_

pipeline {
  agent any
  stages {
    stage("Freezing code") {
      steps {
        script {
          test.gradle()
        }
      }
    }
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'Stage1'
            sleep 60
            echo 'Paso 1 minuto'
          }
        }
        stage('paralelo') {
          steps {
            echo 'testd2'
          }
        }
        stage('paralelo2') {
          steps {
            echo 'testparalelo2'
          }
        }
      }
    }
    stage('stage2') {
      steps {
        echo 'Stage2'
      }
    }
    stage('stage3') {
      steps {
        echo 'Stage2'
      }
    }    
  }
}