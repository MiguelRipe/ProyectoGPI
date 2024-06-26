pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'python -m py_compile app.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
        
    }
}