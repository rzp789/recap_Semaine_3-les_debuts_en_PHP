# Recape S3





# Variables et Conditions  




##Syntaxe: $'nom de la variable' = la 'valeur'et on termine par un ';'



###les valeurs peuvent être de type:

- String (chaine de caracteres)
- Integer (nombre entier)
- Float (nombre décimal)
- Boolean (true ou false) 
- Array (tableau) 
- Object (objet)
- Null (rien)
- Ressource (speciale, fait reference a une ressource externe) 

###Portée des valeurs:

- "Portée globale", écrite dans le script en dessous de l'endroit ou on l'affecte.

- "La portée locale", elle est declarée dans une fonction et elle ne s'applique qu'à l'interieur de la fonction


###Les conditions: 

if / else / elseif / switch / for / while.

Elles donnent des instructions aux programmes:

if (expression) {
// bloc d'instructions 

} elsif (expression){
// bloc d'instructions
}


La condition est evaluée, si elle donne:

- 'true' =>
execute le bloc d'instructions.

- 'false' =>
cherche "else" ou "elseif" pour continuer d'executer le programme.

###Les opérateurs:

- '=' affectation des valeurs.
- '==' égalité (valeur uniquement) 
- '===' égalité (valeur + type)
-  '+' sert a l'addition 
- '%' modulo (reste de la division) 
- '++' ou '--' (sert a l'incrémentation +1 ou la décrémentation -1)
- '||' désigne un 'ou' 
- '&&' désigne un 'et'
- 'switch' : instruction qui permet de tester toutes les valeurs possibles que peut prendre une variable. au même titre que la fonction 'elseif' mais en plus simple et plus facilement lisible. 



## Les Arrays :

* Tableau indéxé numériquement :

    Un tableau indexé numériquement est tout simplement une liste d'éléments repérés chacun par un index numérique unique.
    Un des avantages de ce tabeau est que la clef est attribué automatiquement de 0 à n.
    Ainsi, le premier élément du tableau correspondra à l'index 0, le second à l'index 1, le troisième à l'index 2, etc. 
    Nous noterons bien que la numérotation commence à 0 et non à 1.
    
    exemple : 
                `
                $weapons = ['whip', 'gun', 'saber']
                `
                
* Tableau associatif :

    Un tableau associatif est un tableau dans lequel nous attribuons une valeaur "string, int" à une clef "string".
    
    exemple :   
              
               `$weapons['weapon_one'] = 'whip';
                $weapons['weapon_two'] = 'gun';
                $weapons['weapon_three'] = 'saber';`
                
                ou 
                
                `$weapons = ['weapon_one' => 'whip', 'weapon_two'=>'gun', 'weapon_three'=>'saber'];
                
            
 * Tableau Multidimensionnel : 
 
    Un tableau mutidimensionnel peut contenir en valeur d'autres tableaux. 
    
    exemple : 
    
              `$weapons = [
                      'Indiana Jones' => ['whip', 'gun', 'saber'],
                      'Marion Ravenwood' => ['knife', 'shield'],
                      'Helen Seymour' => ['belt', 'dagger', 'gun', 'shield']
               ]`
              
 
 
 Les tableaux sont les prémices des bases de données qui permettront de classer, trier, stocker .. toutes nos données.
 
 Ils existent un panel de fonctions spécifiques aux traitements des tableaux afin d'utliser leurs données.

Les boucles demandent à PHP de répéter des instructions plusieurs fois.

**while** : à utiliser de préférence lorsqu'on ne sait pas par avance combien de fois la boucle doit être répétée ;

    exemple :
    
        <?php
        	while ($continuer_boucle == true){
        // instructions à exécuter dans la boucle
        	}
        ?>



**for :** à utiliser lorsqu'on veut répéter des instructions un nombre précis de fois.

        exemple :
        
        <?php
	        for ($nombre_de_lignes = 1; $nombre_de_lignes <= 100; $nombre_de_lignes++)
	        {
				 echo 'Ceci est la ligne n°' . $nombre_de_lignes . '<br />';
	        }
	    ?>



**foreach**: est une fonction PHP très pratique. Elle est utilisable pour parcourir un tableau[c'est quoi?]
(ou les membres d'un objet[c'est quoi?]). Il est ainsi possible d'afficher l'ensemble des éléments d'un tableau et les clés associées de la façon suivante:

    <?php
	    foreach ($tableau as $cle => $valeur) {
		    echo $cle.' - '.$valeur.'<br />'."\n";
	    }
    ?>

ou si l'on n'a pas besoin de connaitre les clés

    <?php
	    foreach ($tableau as $valeur) {
    		echo $valeur.'<br />'."\n";
	    }
    ?>

