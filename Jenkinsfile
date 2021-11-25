pipeline {
    agent any

    stages {

        stage('Deploy - Development') {
            when {
                  expression { branch == 'development'}
            }
            steps {
                 echo 'Deploying to development.'
                 echo env.BRANCH_NAME
                
             }
        }
        stage('Deploy - Staging') {
            when {
                 branch 'staging'
            }
            steps {
                 echo 'Deploying to Staging.'
             

             }
        }
        stage('Deploy - Production') {
            when {
                 branch 'main'
            }
            steps {
                 echo 'Deploying to production.'
             }
        }
    }
}
