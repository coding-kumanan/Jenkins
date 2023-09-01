pipeline{
    agent any
    environment{
        GLOBEL = "globel-env"
    }
    stages{
        stage(stage1){
            steps{
                sh "echo Hi from stage1"
            }
        }
        stage(stage 2){
            steps{
                sh "echo ${GLOBEL}"
            }
        }
    }
}