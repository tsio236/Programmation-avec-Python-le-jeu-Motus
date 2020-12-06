# Introduction
  
Dans le cadre du module "*Suite de l'apprentissage de la programmation (Python)*" (**19_E3_IGI_3008_P2**), nous avons eu l'opportunité de réutiliser les notions de Python vues dans le cours pour produire un jeu "Motus" en deux mois. Le travail est réalisé en binôme et l'objectif est de permettre à l'utilisateur de jouer à la phase Lettres du jeu télévisé Motus.  

Notre responsable est Monsieur **Jean-Claude GEORGES**, et notre binôme est composé de Mademoiselle **Andrianihary RAZAFINDRAMISA** et de Mademoiselle **Yovana DENTIKA**.

<br>

As part of the module "*Suite de l'apprentissage de la programmation (Python)*" (**19_E3_IGI_3008_P2**), under the direction of **GEORGES Jean-Claude**, we had the opportunity to reuse the notions of Python seen in the course to produce a game in two months. The work is carried out in pairs and the objective is to allow the user to play the Letters phase of the Motus game show.

Our pair is made of Miss **RAZAFINDRAMISA Andrianihary** and Miss **DENTIKA Yovana**.

<br>

___

# Table des matières / Table of Contents

[[_TOC_]]
___


# Version française

## I. Contexte et règles du motus

### 1. Contexte

Le motus est un jeu issu d’un croisement entre le Mastermind, le jeu de lettres et le bingo.Son but principal est de deviner un mot le plus vite possible afin d’obtenir le plus de points. 

Le jeu oppose un ordinateur et un joueur. Lorsque l’ordinateur est le codeur, le joueur devient le décodeur, et inversement.

Durant une partie classique, l’ordinateur propose un mot de sept lettres fixes (le mot est pris au hasard dans le dictionnaire de l’année en cours), et affiche la première lettre du mot. Le but du joueur est, quant à lui, de deviner le mot en un nombre limité de tentatives, qui varient selon le type de partie, et dans un temps imparti, qui varie également.

Lors de ces multiples tentatives, le joueur propose un mot.

- Si le mot est correct, il gagne la partie.

- Si le mot proposé ne respecte pas les conditions (nombre de lettres, présence dans le dictionnaire), il n’est pas valide et le joueur perd l’une de ses tentatives.

- Si le mot est mal orthographié ou si la proposition faite ne correspond pas au mot fixé par l’ordinateur, les lettres bien placées sont encadrées et illuminées, les lettres présentes dans le mot mais mal placées sont entourées, et si l’une des lettres n’est pas présente dans le mot elle n’est simplement pas mise en avant.

Il y a aussi la possibilité de faire des supers parties de plus de sept lettres. Dans ce cas, l’ordinateur donne plus d’une lettre au début de la partie et le temps est plus long.

Dans le jeu que nous allons initialiser, afin de faciliter la programmation, nous représenterons: en majuscule les lettres bien placées, en minuscule les lettres présentes mais mal placées, et avec des tirets les lettres absentes du mot.

### 2. Objectifs

Lors de l'exécution du jeu, trois types de parties seront possibles:
- La première est basée sur les règles d’origine, le joueur est le décodeur et est censé déterminer le mot fixé par l’ordinateur avec le moins de tentatives possibles.
- La seconde inverse les rôles : le joueur, “codeur”, décide un mot que l’ordinateur devra deviner.L’ordinateur est soumis aux mêmes règles que le joueur.
- Dans la dernière, l’ordinateur est juste un intermédiaire entre deux joueurs. Ces derniers seront concurrents et l’un devra deviner le mot avant son adversaire. Ils jouent dans les mêmes conditions mais sont sur des interfaces différentes. 

Le programme propose également trois niveaux de difficulté et des paramètres variés tels que la langue ou le temps.

De manière générale, le codeur ou le décodeur auront un nombre maximum de huit  tentatives, le programme indiquera au fur et à mesure l’historique des mots proposés et les étapes suivantes. Dans le cas où le joueur est codeur, il lui sera indiqué le format des instructions qu’il devra communiquer à l’ordinateur ( majuscules, minuscules, tirets). 

La première lettre du mot sera toujours donnée et le joueur aura la possibilité de quitter le jeu ou de consulter les règles du jeu à chaque interface. 

A chaque fin de partie, le nombre de coups effectués avant d’avoir trouvé le mot sera décompté et indiqué.

Le mot proposé ou à trouver se trouvera obligatoirement dans le dictionnaire français 2019.

<br>

# English version

## I. Context and rules

### 1. Context

Motus is a game resulting from a cross between Mastermind, Word Game and Bingo. Its main goal is to guess a word as fast as possible in order to get the most points.

The game opposes a computer and a player. When the computer is the encoder, the player becomes the decoder, and vice versa.

During a classic game, the computer suggests a word of seven fixed letters. The word is taken randomly from the dictionary of the current year. The computer displays the first letter of the word and the player's goal is to guess the word in a limited number of attempts - which varies depending on the type of game - and within a given time which varies.

During these multiple attempts, the player suggests a word.

- If the word is correct, he wins the game.

- If the proposed word does not meet the conditions (number of letters, presence in the dictionary), it is not valid and the player loses one of his attempts.

- If the word is misspelled or if it does not correspond to the word fixed by the computer, the well-placed letters are framed and illuminated, the letters present in the word but badly placed are circled, and if one of the letters is not present in the word it is simply not highlighted.

There is also the possibility of making super games of more than seven letters. In this case, the computer gives more than one letter at the start of the game and the time is longer.

In the game that we are going to initialize, in order to facilitate programming, we will represent in uppercase the well placed letters, in lowercase the letters present but badly placed, and with dashes the absent letters.

### 2. Goals

When running the game, three types of games will be possible.

- The first is based on the rules of the original game, the player is the "decoder" and is supposed to determine the word set by the computer with the fewest attempts possible.

- The second type of game reverses the roles: the player becomes the "coder" and decides a word for the computer to guess. The computer is subject to the same rules as the player.

- In the last one, the computer is just an intermediary between two players. They will be competitors and one will have to guess the word before their opponent. They play under the same conditions but are on different interfaces.

The program also offers three levels of difficulty and various settings such as language or time.

Generally, the encoder or decoder will have a maximum number of eight attempts, the program will gradually indicate the history of the history of words that have already been suggested and the following steps. If the player is a "coder", he will be informed of the format of the instructions that he will have to communicate to the computer (upper case, lower case, dashes).

The first letter of the word will always be given and the player will be able to quit the game or consult the rules of the game at each interface.

At each end of the game, the number of moves made before finding the word will be counted and indicated.

The word that the player suggests and that he must find will necessarily be found in a dictionary of the current year.

