pipeline{
agent any
stages{
('fetch code')
{
steps{
git branch :'paac', url: 'https://github.com/devopshydclub/vprofile-project.git'
}
}
stage('build') {
steps{
sh 'mvn install'
}
}
stage('test'){
steps{
sh 'mvn test'
}
}
}
}