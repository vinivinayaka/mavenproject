pipeline {

    agent any

    stages {

        stage('Clean') {

            steps {

                sh 'mvn clean'

            }

        }

        stage('Validate') {

            steps {

                sh 'mvn validate'

            }

        }

        stage('Test') {

            steps {

                sh 'mvn test -DskipTests'

            }

        }

    }

}
