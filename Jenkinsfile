pipeline {
        agent any

        tools {
                maven 'Maven3'
                jdk 'JAVA8'
        }

        stages {
                stage('init') {
                        steps {
                                sh '''
                                        echo "PATH = ${PATH}"
                                        echo "M2_HOME =${M2_HOME}"
                                '''
                        }
                }
                stage() {
                        steps {
                                sh 'mvn install'
                        }
                }
        }
}
