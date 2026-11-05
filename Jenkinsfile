


pipeline {

    agent any

    stages {

        stage('Checkout') {

            steps {

                echo 'Code checked out successfully'

            }

        }

        stage('Run Application') {

            steps {

                bat '"C:\\Users\\STUDENT\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" app.py'

            }

        }

        stage('Run Tests') {

            steps {

                bat '"C:\\Users\\STUDENT\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" test.py'

            }

        }

        stage('Build') {

            steps {

                echo 'Build completed successfully!'

            }

        }

    }

    post {

        success {

            echo 'Jenkins Auto Build Successful!'

        }

        failure {

            echo 'Jenkins Build Failed!'

        }

    }

}
