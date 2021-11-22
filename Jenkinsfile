pipeline {
    agent any

    stages {
        stage('copy fromgit') {
            steps {
                sh 'git clone https://github.com/DanishAnwer1/html-website-templates.git'
            }
        }
        stage('Deploy') {
            steps {
                sh '''cd "/var/lib/jenkins/workspace/github_Sgl_pg_website_pipeline/Animated Landing Page Website Template/" 
                      cp -rf *.* /usr/share/nginx/'''
            }
        }
        stage('Deployed') {
            steps {
                echo 'Deployment '
            }
        }
    }
}
