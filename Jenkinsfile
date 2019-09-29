pipeline {
    agent any
    stages {
        stage ('Initialize') {
            steps {
                /*For windows machine */
                sh
                echo "PATH =${PATH}"
                echo "M2_HOME=${M2_HOME}"

                /*For Mac & Linux machine */
               // sh  'mvn clean package'
            }

        }

        stage ('Deploy Build in Staging Area'){
            steps{

                build job : 'Deploy-StagingArea-Piple'

            }
        }

        stage ('Build'){
            steps{
                echo 'Hello World'
                }
                
            }
            }
        }
    }
}
