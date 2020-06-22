node{
    
      stage('Checkout source code from git'){
        git url: 'https://github.com/cgghali/ci-cd-demo.git', branch: 'master'
      }
      
      stage('Maven clean Package'){
          def mavenhome = tool name: "Maven-3.7.0", type: "maven"
          def mavenCMD = "${mavenhome}/bin/mvn"
          sh "${mavenCMD} clean package"
  }
}
