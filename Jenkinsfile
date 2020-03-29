pipeline {
         agent tout 
          
   étapes {
       étape ( ' Build ' ) {
           pas {
                    withMaven ( Maven : ' maven-3.6.3 ' ) {
            
               sh ' mvn clean compile '
                    }
           }
       }
       étape ( ' Test '  ) {
           pas {
                    withMaven ( Maven : ' maven-3.6.3 ' ) {
                    
               sh ' test mvn '
           }
       }
   }
        étape ( ' déployer ' ) {
           pas {
                    withMaven ( Maven : ' maven-3.6.3 ' ) {
                    
               sh ' mvn deploy '
           }
       }
   }     
}
         }
