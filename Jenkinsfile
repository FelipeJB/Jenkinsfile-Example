pipeline {
    agent {
        label "master"
    }
    
    environment {
        firstEmployee = "Felipe"
        secondEmployee = "Juan"
        thirdEmployee = "Jose"
    }    

    parameters {
        text(name: 'BOSS_NAME', defaultValue: 'MARTIN', description: 'Name of the Boss')
    }

    stages {
        stage ('Execution') {
            parallel {
                stage ('First Employee Tasks') {
                    agent any
                    steps{
                        script {
                            echo "${params.BOSS_NAME} sent ${firstEmployee} to count from 1 to 4: 1"
                            echo "${params.BOSS_NAME} sent ${firstEmployee} to count from 1 to 4: 2"
                            echo "${params.BOSS_NAME} sent ${firstEmployee} to count from 1 to 4: 3"
                            echo "${params.BOSS_NAME} sent ${firstEmployee} to count from 1 to 4: 4"
                        } 
                    }
                }

                stage ('Second Employee Tasks') {
                    agent any
                    steps{
                        script {
                            echo "${params.BOSS_NAME} sent ${secondEmployee} to count from 1 to 4: 1"
                            echo "${params.BOSS_NAME} sent ${secondEmployee} to count from 1 to 4: 2"
                            echo "${params.BOSS_NAME} sent ${secondEmployee} to count from 1 to 4: 3"
                            echo "${params.BOSS_NAME} sent ${secondEmployee} to count from 1 to 4: 4"
                        } 
                    }
                }
                
                stage ('Third Employee Tasks') {
                    agent any
                    steps{
                        script {
                            echo "${params.BOSS_NAME} sent ${thirdEmployee} to count from 1 to 4: 1"
                            echo "${params.BOSS_NAME} sent ${thirdEmployee} to count from 1 to 4: 2"
                            echo "${params.BOSS_NAME} sent ${thirdEmployee} to count from 1 to 4: 3"
                            echo "${params.BOSS_NAME} sent ${thirdEmployee} to count from 1 to 4: 4"
                        } 
                    }
                }
            }
        }
    }
    
}   
