pipeline {
    agent any

    stages {
        stage('copy from git') {
            steps {
                sh 'git clone https://github.com/DanishAnwer1/html-website-templates.git'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cp -rf *.* "/var/lib/jenkins/workspace/github_Sgl_pg_website/Animated Landing Page Website Template" /usr/share/nginx/html'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment '
            }
        }
    }
}
