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
 
 
 
 
