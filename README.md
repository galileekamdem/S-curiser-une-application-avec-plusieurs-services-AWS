# S-curiser-une-application-avec-plusieurs-services-AWS
Sécuriser une application  avec plusieurs services AWS
🔐 Sécuriser une application avec plusieurs services AWS
Ce projet est un laboratoire pratique conçu pour démontrer comment renforcer la sécurité d’une application déployée sur AWS en intégrant plusieurs services de sécurité cloud. Il simule une mission dans laquelle vous intervenez comme administrateur SysOps pour une entreprise novice en AWS.

🚀 Objectifs du projet
Supprimer les secrets sensibles d’un modèle CloudFormation

Mettre en place une Web ACL via AWS WAF

Configurer une instance EC2 compatible avec AWS Systems Manager

Activer Amazon Inspector pour l’analyse de vulnérabilités

Consolider la posture de sécurité avec AWS Security Hub

Stocker les secrets d’une base de données via AWS Secrets Manager

🛠️ Services AWS utilisés
Amazon EC2

AWS CloudFormation

AWS WAF

AWS Secrets Manager

Amazon Inspector

AWS IAM

AWS Config

AWS Security Hub

🧩 Architecture
L’architecture repose sur une application WordPress déployée avec CloudFormation, protégée par un Application Load Balancer, avec une base de données Amazon RDS en backend. Les règles WAF sécurisent l’entrée, tandis que l’ensemble des services de sécurité AWS renforcent la visibilité, la détection et la gestion des vulnérabilités.

Utilisateur → ALB → EC2 (WordPress) → RDS  
       ↘︎ AWS WAF  
       ↘︎ Amazon Inspector  
       ↘︎ Secrets Manager  
       ↘︎ Security Hub
✅ Étapes réalisées
Déploiement avec CloudFormation Déploiement d’une stack WordPress avec paramètres personnalisés.

Stockage des secrets Utilisation de Secrets Manager pour stocker les identifiants RDS.

Création d’une Web ACL Application de règles gérées (OWASP, SQLi, Bad Inputs) à l’ALB.

Configuration EC2 avec SSM Attribution d’un rôle IAM avec la politique AmazonSSMManagedInstanceCore.

Activation des outils de sécurité

Amazon Inspector

AWS Security Hub avec AWS Config

📦 Nettoyage des ressources
💡 Pensez à supprimer toutes les ressources à la fin du laboratoire pour éviter toute facturation hors free tier.

✍️ Auteur
Projet réalisé par Kevin — passionné par la sécurité cloud, AWS et la création de contenus techniques accessibles et engageants.
