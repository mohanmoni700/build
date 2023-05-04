pipeline {
agent any
  stages {
    stage('git checkout') {
      steps {
        sh '''
        echo "clonning the app repo"
        '''
        checkout([$class: 'GitSCM',
                  branches: [[name: 'main']],
                  userRemoteConfigs: [[url: 'https://github.com/mohanmoni700/build/tree/main/maven_app']]])
      }
    }
  }




}
