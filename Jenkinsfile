pipeline {
agent any
  stages {
    stage('git checkout') {
      steps {
        sh '''
        echo "clonning the app repo"
        '''
        git branch: 'main' , url: 'https://github.com/mohanmoni700/build/tree/main/maven_app/'
    }
  }
 }




}
