node
{
    stage('Initialization')
    {
        sh 'echo dummy stage'
        sh 'sleep 20'
    }
}
stage('Testing')
{
    parallel centos: 
    {
        node ('centos')
        {
            sh 'echo Hellofrom Centos'
            sh 'sleep 30'
        }
    }
    ubuntu
    {
        sh 'echo Hellofrom Ubuntu'
         sh 'sleep 30'

    }
}