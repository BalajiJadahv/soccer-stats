#!groovy​

// FULL_BUILD -> true/false build parameter to define if we need to run the entire stack for lab purpose only
//final FULL_BUILD = params.FULL_BUILD
// HOST_PROVISION -> server to run ansible based on provision/inventory.ini
//final HOST_PROVISION = params.HOST_PROVISION

//final GIT_URL = 'https://github.com/BalajiJadahv/soccer-stats.git'
//final NEXUS_URL = 'nexus.local:8081'
pipeline{
agent any

stages{
    stage('Checkout Code') {
              //  node {
          steps{  
               git 'https://github.com/BalajiJadahv/soccer-stats.git'
              }
           }
    
   
    stage('Build Stage'){
             steps{
        //       withMaven(maven : 'maven_3_3_9'){
        //       sh "mvn -B versions:set -DnewVersion=${pom.version}-${BUILD_NUMBER}"
       //        sh "mvn -B -Dmaven.test.skip=true clean package"
      //         stash name: "artifact", includes: "target/soccer-stats-*.war"
      //     }
    // }
       sh 'mvn clean compile'
}   
}
}
}
//}
//}
//if(FULL_BUILD) {
 //   stage('Unit Tests') {   
  //      node {
  //          withEnv(["PATH+MAVEN=${tool 'MAVEN_HOME'}/bin"]) {
    //            sh "mvn -B clean test"
    //            stash name: "unit_tests", includes: "target/surefire-reports/**"
    //        }
     //   }
   // }
//}

//if(FULL_BUILD) {
  //  stage('Integration Tests') {
    //    node {
      //      withEnv(["PATH+MAVEN=${tool 'MAVEN_HOME'}/bin"]) {
    //            sh "mvn -B clean verify -Dsurefire.skip=true"
        //        stash name: 'it_tests', includes: 'target/failsafe-reports/**'
         //   }
       // }
  //  }
//}
//}
//}
