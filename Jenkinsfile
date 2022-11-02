pipeline {  

    agent any  

    stages {  

            stage ('Clean') {

                steps {  

                        sh 'mvn clean'

                }  

            }  

           stage ('Validate') {

                steps {  

                        sh 'mvn validate'

                }  

            }

              stage ('Test') {

                steps {  

                        sh 'mvn test -DskipTests'

                }  

            }  

              stage ('Package') {

                steps {  

                         sh 'mvn package -DskipTests'

                }  

            }  

            stage ('Verify') {

                steps {  

                         sh 'mvn verify -DskipTests'

                }  

            }  

            stage ('Install') {

                steps {  

                         sh 'mvn install -DskipTests'

                }  

            }  

    }  

}  
