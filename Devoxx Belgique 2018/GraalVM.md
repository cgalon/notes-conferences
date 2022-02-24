#GraalVM 

Automatic transformation of interpreters to compilers  
Engine integration native and managed  
  
Remplace le JIT compiler par Graal compiler (écrit en Java)  
Optimise le code compilé produit  
  
Github → oracle/graal  
  
Community edition et Enterprise edition  
  
Moins efficace sur des frameworks car le code est déjà optimisé.  
  
Permet aussi de générer du code exécutable → native-image  
Mélange le code de la JVM et le code fonctionnel dans un executable  
Par défaut effectue les initialisations statiques à la génération. Mais peut être reporté au runtime  
Toutes les features de #Java ne sont pas encore supportées (dynamic classloading, reflexion...)  
→ pas de limitations sur le compilateur de GraalVM, juste sur les native-images

[https://www.graalvm.org/](https://www.graalvm.org/)