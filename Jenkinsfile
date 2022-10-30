pipeline{
    agent{
         label{
           label 'built-in'
}
}
    stages{
      stage('install httpd'){
           steps{
                sh"yum install httpd -y"
}
}
      stage('start httpd'){
        steps{
         sh"service httpd start"
}
}
      stage('deploy httpd'){
        steps{
          sh"copy index.html /var/www/html"
}
}
}
}
