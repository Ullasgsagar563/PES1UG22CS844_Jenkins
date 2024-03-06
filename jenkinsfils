pipeline{
  agent any
  stages{
    stage('Build'){
steps{
build 'PES1UG22CS844-1'
sh 'g++ main.cpp -o output'
}
}
stage('Test'){
strps{
sh './output'
}
}
stage('Deploy'){
steps{
echo 'deploy'
}
}
}
post{
failure{
error 'pipline failed'
}
}
}
