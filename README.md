# L1_Projet_SamTest
SAMTEST


OBJECTIFS DU PROJET

La réouverture des bars et restaurants approchant, les regroupements massifs et précipités vont se produire. Il est donc essentiel de mesurer la quantité d’alcool présente dans l’air expiré pour savoir s’il est possible ou non de prendre le volant. 
Conduite sous l’emprise d’alcool = 1ère cause de mortalité sur les routes  
Davantage pratique d’obtenir le résultat par un son ou un LED que par la lecture d’une quantité.
 Si le bruit retentit et que les LED deviennent rouges, le taux d’alcoolémie est supérieur au seuil autorisé. 
     A l’inverse, si aucun bruit ne se manifeste et que les LED deviennent vertes, le test est considéré comme négatif. 
     
     
DIFFERENTS BLOCS FONCTIONNELS DU PROJET 

Le capteur est relié à la carte Arduino par trois branchements :
 Un relié à l’entrée Analog In A0
 Un relié à l’alimentation 3.3V 
 Le dernier relié au GND de l’Arduino  
A l’intérieur du capteur, un dispositif fait varier la tension (au VCC) et sera lue par l’entrée Analog In
AnalogRead convertit la tension en valeur numérique qu’on pourra exploiter pour l’afficher sur un traceur série et déclencher une alarme si la valeur lue est supérieure au seuil que nous avons rentré dans le programme. La valeur du seuil est fixé à 20 ici. 
Une fois le code téléversé, nous ouvrons le traceur série. Au repos, sans détection de fumée et vapeur d’alcool, la valeur est comprise entre 4 et 5. Il n’ya pas besoin de boire beaucoup pour que le capteur réagisse, une gorgée suffit. Lors du test, la valeur est maintenant égale à 40.

PLAN D’EXECUTION

Schéma du circuit (branchements)
Réalisation des branchements entre la carte et le capteur
Rédaction du code (établissement du seuil, if, AnalogRead…)
Lecture sur le traceur série
Mise en place d’un buzzer pour alerter le dépassement du seuil
Nouveaux branchements
Création d’un tube et d’une boite à ouvertures avec l’imprimante Ultimaker 3

MATERIEL UTILISE

Capteur MQ135 : Module de détection de gaz, qualité de l’air
Buzzer d’alarme (sonore continu)
Carte Arduino pro mini
Fils, LED
Tube à utiliser lors du soufflement
Imprimante 3D Ultimaker 3
Boite Samtest couvrant la carte et les branchements

CE QU’ON AURAIT PU FAIRE

  A la suite des résultats, permettre ou non l’accès au véhicule, ainsi, si le conducteur est testé positif, il ne pourrait pas ouvrir la voiture. Ou faire en sorte de ne pas pouvoir démarrer après la réalisation du test, le système étant relié au faisceau électrique du véhicule.
  
  PROBLEMES RENCONTRES
  
   La forte sensibilité du capteur a nécessité un calibrage et nous avons du recommencé les impressions des objets suite à des soucis techniques de l'imprimante.

