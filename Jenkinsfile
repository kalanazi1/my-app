pipeline {
    agent any 
    }
    stage('Build') {
        def mvn_version = 'M3'
        withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ) {
        sh '''for f in i7j-*; do
                (cd $f && mvn clean package -Dmaven.test.skip=true -Dadditionalparam=-Xdoclint:none  | tee ../jel-mvn-$f.log) &
              done
              wait'''
        }
   }
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
