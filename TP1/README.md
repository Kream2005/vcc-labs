# TP1 : De la machine au conteneur

## Étape 1

1. Une machine virtuelle est une instance logique qui utilise des ressources virtualisées (CPU, RAM, stockage).
2. Isolation importante, ce qui améliore la sécurité. Optimisation des ressources en hébergeant plusieurs machines virtuelles sur une même machine physique.
3. Une VM permet d'exécuter plusieurs applications nécessitant des environnements différents sur une même machine physique. Contrairement à une utilisation directe de l'ordinateur, elle n'a pas un accès direct aux ressources physiques, car celles-ci sont gérées et partagées par l'hyperviseur.

## Étape 2

1. Un conteneur Docker est un environnement isolé créé à partir d'une image Docker. Il exécute une application et ses dépendances dans un environnement indépendant.
2. Les conteneurs utilisent le système d'exploitation de la machine hôte, alors que les VM possèdent leur propre système d'exploitation. Ils sont donc plus légers et plus rapides à démarrer.
3. Ils sont légers, facilement reproductibles et adaptés aux architectures modernes, notamment aux microservices.

## Étape 3

1. Le Dockerfile crée une image de manière automatisée et reproductible, sans risque d'erreur humaine lors d'une configuration manuelle.
2. Une image est un modèle contenant le système de fichiers, le code, les dépendances et ce qui est nécessaire à l'exécution. Un conteneur est une instance en cours d'exécution de cette image.

## Étape 4

1. Une seule commande construit, lance et arrête tous les services, et le réseau qui les relie est créé automatiquement, au lieu de gérer chaque conteneur un par un.
2. Il décrit toute l'application (services, ports, réseaux) : c'est la configuration du déploiement, versionnable dans Git.
3. Limites : déploiement sur plusieurs machines, haute disponibilité, montée en charge automatique. Un orchestrateur comme Kubernetes est alors plus adapté.