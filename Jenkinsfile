pipeline
{
agent any
stages
{
stage("version checking")
{
steps{
sh "php --version"
}
}
stage("running php code")
{
steps{
sh "php hello.php"
}
}

}}
