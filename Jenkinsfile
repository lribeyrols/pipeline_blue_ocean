pipeline {
  agent {
    node {
      label 'New change'
    }
    
  }
  stages {
    stage('Qualification') {
      steps {
        build(job: 'MI', propagate: true)
      }
    }
    stage('Edition bon de commande') {
      steps {
        mail(subject: 'test ok', body: 'le test est ok')
      }
    }
    stage('Implémentation ') {
      steps {
        mail(subject: 'test ok', body: 'le test est ok')
      }
    }
    stage('Test') {
      steps {
        mail(subject: 'test ok', body: 'le test est ok')
      }
    }
    stage('End') {
      steps {
        node(label: 'End')
      }
    }
  }
}