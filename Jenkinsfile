pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/riti-1904/my-jenkins-project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt || echo "No dependencies needed"'
            }
        }

        stage('Run Script') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
