# Gherkin-ast

**Gherkin** ye un llinguaxe informáticu pa diseñar pruebes de programes d'ordenador.

**Gherkin** básase nel llinguaxe natural pa que seya fácil de entender pol
cliente, que non tien que entender un llinguaxe de programación complexu.

Les carauterístiques del proyeutu escríbense de forma que sirven pa xenerar
les pruebes de que tó furrula correutamente, y tamén puen entendese comu el
contratu o acuerdu entre el desarrollaor y el cliente.

N'inglés una carauterística del proyeutu en Gherkins tien esti aspeutu:

```gherkin
Feature: Listing command
  In order to change the structure of the folder I am currently in
  As a UNIX user
  I need to be able see the currently available files and folders there

Scenario: Listing two files in a directory
  Given I am a directory "test"
  And I have a file named "foo"
  And I have a file named "bar"
  When I run "ls"
  Then I should get:
    """
    bar
    foo
    """
```

L'oxetivu d'esti proyeutu ye poder escribir estes carauterístiques n'Asturianu
d'un modu asemeyau a este:

```
Carauterística: Comandu llistar
  Pa ser capaz muda'l xeitu de la carpeta na que toi
  Comu usuariu UNIX
  Teo de ser capaz ver los ficheros y carpetes que hai nella

Casu: Llistar dos ficheros nuna carpeta
  Dáu que toi nuna carpeta "test"
  Y que teo un ficheru nomáo "foo"
  Y que teo un ficheru nomáo "bar"
  Cuando executo "ls"
  Entós debo tener:
    """
    bar
    foo
    """
```

## Contribuyir 
Esti proyeutu entámase pa crear el fichero de llinguaxes de Gherkin metió
n'asturianu, esplicar pa que val, y'aldericar de la traducción, etc.

Una vegada que tea fecho hai que añedílo nel ficheru de llinguaxes del
proyeutu `cucumber/gherkin` y pedí-yos (*pull request*) qu'acepten los
cambeos.

## Sides
Nun soi asturianu parlante, soi charnegu/maketu/foriatu andaluz ensin educación
 formal en llingua asturiana. To lo más críeme en Grao, lleí les Croniques de
 Leodegundu fai 15 años, y préstanme los cancios y lleélo dacuando. 

Esti testu nun pudo escríbise ensin l'ayuda del [Diccionario General de la
Lengua Asturiana](http://mas.lne.es/diccionario/) (sic - en castellán nel
orixinal) de La Nueva España; y de
[Eslema](http://di098.edv.uniovi.es/apertium/comun/traductor.php) el tradutor
automáticau desenvueltu pela Universidá d'Uviéu.

Si atopas dalgún erru, ye la mio culpa, y prestárame asgaya incluyir les vueses
correciones.

