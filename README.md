# MySQL
## Présentation 
MySQL est un système de gestion de bases de données relationnelles (SGBDR). Il est distribué sous une double licence GPL et propriétaire. Il fait partie des logiciels de gestion de base de données les plus utilisés au monde, autant par le grand public (applications web principalement) que par des professionnels, en concurrence avec Oracle, Informix et Microsoft SQL Server.

Son nom vient du prénom de la fille du cocréateur Michael Widenius, My. SQL fait allusion au Structured Query Language, le langage de requête utilisé.

Le nom du logo de MySQL (le dauphin) Sakila, a été choisi par les créateurs de MySQL sur la base d'un concours.

## Language SQL

SQL (sigle de Structured Query Language, en français langage de requête structurée) est un langage informatique normalisé servant à exploiter des bases de données relationnelles. La partie langage de manipulation des données de SQL permet de rechercher, d'ajouter, de modifier ou de supprimer des données dans les bases de données relationnelles.

## Syntaxe générale

Les instructions SQL s'écrivent d'une manière qui ressemble à celle de phrases ordinaires en anglais. Cette ressemblance voulue vise à faciliter l'apprentissage et la lecture.

### Exemple de code
 - Modification d'une table
```sql
ALTER TABLE `table1` ADD COLUMN `colonne5` INTEGER NULL;
```
 - Recherche
```sql
SELECT `nom`, `service`
FROM `employe`
WHERE `statut` = 'stagiaire'
ORDER BY `nom`;
```
 - Insère des lignes dans une table existante
```sql
INSERT INTO `a_table` (`field1`, `field2`, `field3`)
VALUES ('test', 'N', NULL);
```
 - Modifie un ensemble d'enregistrement existant dans une table
```sql
UPDATE `a_table`
SET `field1` = 'updated value'
WHERE `field2` = 'N';
```
 - Supprime un enregistrement existant dans une table
```sql
DELETE FROM `a_table`
WHERE `field2` = 'N';
```
PHP offre 3 APIs différentes pour se connecter à MySQL. (mysql, mysqli et PDO)

Quel API choisir ? https://secure.php.net/manual/fr/mysqli.overview.php

## API MySQL originale
Cette extension est obsolète depuis PHP 5.5.0 et n'est pas recommandée pour écrire vos nouvelles lignes de code, sachant qu'elle sera supprimée dans un futur proche. A la place, soit l'extension mysqli ou PDO_MySQL devrait être utilisée.

## Extension mysqli
L'extension mysqli vous permet d'accéder aux fonctionnalités fournies par MySQL 4.1 et supérieur.
L'extension propose une interface orientée objet et aussi une interface procédurale.

### Fonction

  

Référence :
	- Site Officiel : http://www.mysql.com/
	- Documentation Officiel : http://dev.mysql.com/doc/
  - Statistique d'utilisation : http://db-engines.com/en/ranking
  - Cours et tuto : http://sql.sh
