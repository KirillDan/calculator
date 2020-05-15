pipeline {
    agent any
    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/KirillDan/calculator'
            }
        }
        stage("Compile") {
            steps {
                 sh " ./mvnw compile"
            }
        }
        stage("Unit test") {
            steps {
              sh "./mvnw test"
            }
        }
    }
}
