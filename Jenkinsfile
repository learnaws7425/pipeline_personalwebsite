pipeline {
   agent any

   stages {
      stage('install') {
         steps {
            echo 'Downloading the Code'
            git url: 'https://github.com/learnaws7425/personalWebSite.git'
            sh "whoami"
            sh "sudo yum install -y apache2"
            echo 'Installed the code and Starting the RUN'
         }
      }
       stage('run') {
         steps {
            echo 'In running State'
            echo 'Current Folder'
            sh "pwd"
            sh "sudo cp -r * .  /var/www/html/"
         }
      }
       stage('deploy') {
         steps {
            echo 'Will deploy the site now'
         }
      }
   }
}
