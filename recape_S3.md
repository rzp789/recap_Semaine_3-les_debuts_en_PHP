# Recape S3

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






