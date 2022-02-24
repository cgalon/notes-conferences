#Java

Split en 3 modules.  
#JUnit Vintage pour rétrocompatbilité  
JUnit Jupiter → Le nouveau JUnit  
JUnit plateform → Pour intégration avec les IDE (pas besoin pour IntelliJ)  
  
Renommage des annotations (BeforeXXX, AfterXXX, ...)  
  
Ajout d'assertions  
assertThrows pour tester la levée des exceptions  
assertAll pour ne pas s'arrêter à la première erreur  
  
#tests paramétrés (@ParametrizedTest, @ValueSource, @CsvSource)  
  
@ExtendsWith pour remplacer les runners (Spring par exemple) par des extensions  
  
@DisplayNameGenerator pour transformer les noms des tests dans le message du reporting  
  
Possibilité d'injecter des valeurs via des ParameterResolvers  
  
[https://gitlab.com/crafts-records/remember-me](https://gitlab.com/crafts-records/remember-me)