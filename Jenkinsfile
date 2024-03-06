pipeline {
    agent any
    parameters {
           choice choices: ['DEV', 'TEST', 'PROD'], description: 'This is environment to be deployed ', name: 'Envionment_name'
          string defaultValue: 'builduser', description: 'Username required for environment deployment', name: 'useranme'
         }
    stages{
        stage("build code"){
            steps{
                sh " echo build"
        }
        }
        stage("create package"){
            steps{
                sh " echo package"
          }
        }
        stage("package upload"){
            steps{
                sh " echo upload"
          }
        }
        stage("sonarqube scan"){
            steps{
                sh " echo scan"
          }
        }
        stage("deployment on TEST enviornment"){
            steps{
                sh " echo TEST "
          }
        }
}
}