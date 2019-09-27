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
