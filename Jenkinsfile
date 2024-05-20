pipeline
{
agent {
        docker { image 'my-php-app' }
    }
stages
{
stage("version checking")
{
steps{
sh "docker run my-php-app"
}
}


}}
