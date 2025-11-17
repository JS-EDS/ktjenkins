pipeline {
  agent any
  stages {
    stage('git clone or git pull in myself') {
      steps {
        git url: 'https://github.com/JS-EDS/ktjenkins.git'. branch: 'master'
      }
    }
    stage('CD using K8s in myself'){
      steps {
        sh '''
	kubectl applty -f testapp.yml
	'''
      }
    }
  }
}
