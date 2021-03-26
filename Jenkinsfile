pipeline{

agent any
    tools {
         maven "maven"
          }

stages {
  
    stage('git checkout'){

    steps {

      git 'https://github.com/devikaranimuddana/hello-world-sc.git'
          } 
                         }   
   stage('compile and build step'){
    
    steps {
     
      echo "Building java code is in progress..."

      sh "mvn -Dmaven.test.failure.ignore=true clean package" 

          }      
                                    }
    stage('Deploy war file to Tomcat container'){

     steps {

       sh 'curl --upload-file /var/jenkins_home/workspace/DevOps_Pipeline/webapp/target/*.war "http://tomcat:tomcat@34.66.211.121:8082/manager/text/deploy?path=/myapp&update=true"'
    

           }
						}


         }      
         }  

