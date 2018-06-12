pipeline {
  agent any
  stages {
    stage('Primer paso') {
      steps {
        echo 'Primer paso'
        jiraComment(issueKey: 'SCRUM-1', body: 'Este es un comentario añadido desde Jenkins')
      }
    }
    stage('Pasos Paralelos') {
      parallel {
        stage('Segundo primer paso') {
          steps {
            echo 'paso 2.1'
          }
        }
        stage('Segundo segun paso') {
          steps {
            echo 'paso 2.2'
          }
        }
      }
    }
    stage('Tercer paso') {
      steps {
        echo 'Paso 3'
      }
    }
  }
}