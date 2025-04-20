pipeline {
    agent any
    stages {
        stage('Install dependencies') {
            steps {
                sh 'python3 -m pip install -r requirements.txt'
            }
        }
        stage('Run tests') {
            steps {
                sh 'python3 -m pytest tests/ --maxfail=1 --disable-warnings -q'
            }
        }
    }
}
