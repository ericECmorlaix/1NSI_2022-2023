# Mon Notebook
## Chaines :

Ex: 

'hello'

mot = hello   
guillemets = indique que c´est une chaine de caractères

Possibilité d´additionner des chaines

Ex: 

'hello' + 'world'

## Variables :

Ex: 

mot = 'hello'  

--> 
  hello   
  
  
  car la variable mot est définie
  
  
Ex: 

soleil 

--> 
  erreur   
  
  car la varaible soleil n´est pas définie, Python cherche sa valeur

Ex:

mot = 'hello'  

votre_nom = Lennie  

print(mot + ' ' + votre_nom) 

--> 
  hello Lennie

## Boucle for :

for <variable> in <itérable> : <code à repéter>
Ex: 
  
nom : 'world'   
  
ligne = '-'  
  
for caractere in nom: 
  
   print(ligne + nom)
                                    
  --> 
  
  -world
  
  -world
  
  -world
  
  -world
  
  -world
  
## Construction de chaines :
  
Ex: 
  
nom = 'World'   
  
ligne = ' '    
  
for caractere in nom:
  
    ligne = ligne + caractere
  
    print(ligne)
  
-->

  W
  
  Wo
  
  Wor
  
  Worl
  
  World
  
On peut aussi modifier le script pour que les caractères soient inversés :
  Il suffit d´inverser caractere et ligne dans <ligne = ligne + caractere> ce qui donnerais <ligne = caractere + ligne>
  
Ex: 
  
nom = 'World'   
  
ligne = ' '   
  
for caractere in nom:
  
    ligne = caractere + ligne
  
    print(ligne)
  
-->
  
  W
  
  oW
  
  roW
  
  lroW
  
  dlroW

Au passage, le caractere _ dans une boucle tel que for caractere in ...: est égale à caractere, on peut donc le remplacer par _. Cela ne change pas l'exécution du script, mais est utile au lecteur.

## Structures conditionnellles :
  
Les deux seuls booléens: True et False.
Les booléens sont généralement utilisés dans des structures if, quand l'ordinateur voit if <condition>:, il vérifie si <condition> est vraie (True). 
  
Si c'est le cas, il exécute le corps : un bloc d'instructions. Sinon, il l'évite et passe à la suite du script.
  
Ex:
  
phrase = 'Hello World'
  
ravi = True
  
if ravi:
  
    phrase += '!'
  
print(phrase)
  
--> 
  
  Hello World!
  
car ravi est vrai(True), mais si on change True en False comme ceci:
  
Ex:
  
phrase = 'Hello World'
  
ravi = True
  
if ravi:
  
    phrase += '!'
  
print(phrase)
  
-->
  
  Hello World
  
car ravi est faux, l´ordinateur n´execute pas la boucle if.
  
## Structures imbriquées :
  
Les structures de contrôle for ou conditionnelles if comportent un bloc d'instructions internes.
  
Ex d'une boucle for à l'intérieur d'une structure if :
  
phrase = 'Hello World'
  
ravi = True

if ravi:
  
    nouvelle_phrase = ''
  
    for caractere in phrase:
  
        nouvelle_phrase += caractere + '!'
  
    phrase = nouvelle_phrase
    
print(phrase)
  
-->
  
  H!e!l!l!o! !W!o!r!l!d!
  
Il est aussi possible de créer une structure if à l´intérieur d´un boucle for.
  
## If et else :
  
Le bloc else est comme un « ou sinon ... » : si la condition du if n'est pas respectée, alors les instructions dans le bloc else seront exécutées. Que la condition soit vérifiée ou non, l'un ou l'autre des deux blocs sera obligatoirement exécuté.
  
Ex:
  
condition = True
  
if condition:
  
    print('Oui')
  
else:
  
    print('Non')
  
--> 
  
  Oui
  
car le bloc if est vérifié. Mais si on change True par False comme ceci :
  
condition = False
  
if condition:
  
    print('Oui')
  
else:
  
    print('Non')
  
-->
  
  Non
  
On peut donc voir que le programme execute le bloc else car le bloc if n´est pas vérifié.
  
