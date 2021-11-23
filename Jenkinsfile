pipeline {
    agent any

    stages 
    {
        stage('removing previous build') {
            steps {
                sh '''cd /var/lib/jenkins/workspace/github_Sgl_pg_website_pipeline/ 
                    rm -rf *'''
            }
        }
        stage('copy fromgit') {
            steps {
                sh 'git clone https://github.com/DanishAnwer1/html-website-templates.git'
            }
        }
        stage('Deploy') {
            steps {
                sh '''cd "/var/lib/jenkins/workspace/github_Sgl_pg_website_pipeline/html-website-templates/Animated Landing Page Website Template" 
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
