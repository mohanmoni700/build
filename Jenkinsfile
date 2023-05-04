pipeline {
  agent any
      stages {
                stage('git checkout') {
                            steps {
                                                  sh '''
                                                  echo "clonning the app repo"
                                                  '''
                                                  git branch: 'main' , url: 'https://github.com/mohanmoni700/build.git'
                            }
                }

                stage('compile and build') {
                            steps {
                                                sh '''
                                                cd /var/jenkins_home/workspace/maven-app
                                                '''
                                                mvn clean install
                            }
                }            

       }

}
