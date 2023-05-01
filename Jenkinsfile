pipeline
{
    agent any
    stages
    {
        stage('clean')
        {
            steps
            {
                sh 'rm -r *'
                sh 'rm -r ../../../../www/html/*'
            }
        }
        stage('clone')
        {
            steps
            {
                sh 'git clone https://gitlab.com/1rn19is401.deepika/jenkins-webproject.git -b master'
            }
        }
        stage('deploy')
        {
            steps
            {
                sh 'mv web2/* ../../../../www/html'
            }
        }
    }
}