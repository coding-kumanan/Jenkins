pipeline {
    agent any
    environment{
        GLOBEL = "globel-env"   //pipeline variable:All the stages can acces this
    }
    stages{
        stage('stage 1'){
            steps{
                sh "echo hello world-stage 1"
                sh "echo stage 1 shell comment"
                sh "echo globel env variable is ${GLOBEL}"
            }
        }
        stage('stage 2'){
            environment{
                GLOBEL = "batch55"  //stage level variable: inside the stage can acces it will overide pipeline variable
                }
                steps{
                    sh "echo stage 2 hai"
                    sh "echo stage 2 shell comment"
                    sh "echo batch name is ${GLOBEL}" 
                }
            }
            stage('stage 4'){
                steps{
                    sh ''' echo stage-3 hai
                           echo stage-3 shell comment
                           pwd
                        '''                 
                }
            }
        

    }
} 
