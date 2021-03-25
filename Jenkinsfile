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

      sh "mvn -Dmaven.test.failure.ignore=true clean package" 



}
}


}
}

