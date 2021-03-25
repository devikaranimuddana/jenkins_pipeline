pipeline{

agent any

stages {
  
    stage('git checkout'){

    steps {

      git 'https://github.com/devikaranimuddana/hello-world-sc.git'
}
}
   stage('compile and build step'){
    
    steps {
     
      echo "Building java code is in progress..."

      sh '/usr/local/hello-world-sc'
      sh "mvn -Dmaven.test.failure.ignore=true clean package" 



}
}


}
}

