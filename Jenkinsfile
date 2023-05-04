pipeline {
agent any
  stages {
    stage('git checkout') {
      steps {
        sh '''
        echo "clonning the app repo"
        '''
        checkout([$class: 'GitSCM',
                  branches: [[name: 'master']],
                  userRemoteConfigs: [[url: 'https://github.com/mohanmoni700/build.git']]])
      }




}
