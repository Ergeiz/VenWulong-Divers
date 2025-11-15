# Question à Gemini
> Dans le cadre du jeu Guild Wars sur PC en multi boxing, on utilise l'application GWMultiLaunch pour lancer
>  nos différents comptes de jeu en même temps.  
> Certains utilisent aussi une application tierce, la GWToolbox++ .  
> Quelques personnes ont rencontrés quelques soucis les derniers temps:  
> ils lançaient plusieurs comptes du jeu et se retrouvaient "bloqué" sur l'un (le ALT+TAB pour passer d'un compte
> à l'autre ne marchait pas) et rencontraient des soucis de clavier.  
> Pour ceux ayant rencontré ce problème, ils étaient des utilisateurs habituel de la GWToolbox++, mais ne l'utilisaient pas forcement à ce moment là.  
> Fais moi une recherche sur ce problème.

# Réponse de Gemini
Bonjour \!

J'ai effectué des recherches concernant ce problème spécifique de blocage "Alt+Tab" et de soucis clavier lors de l'utilisation de **GWMultiLaunch** dans un contexte où **GWToolbox++** est ou a été utilisé.

Voici la synthèse des informations trouvées :

### 🚩 L'incompatibilité principale identifiée

Le point le plus important découvert est que **GWToolbox++ déconseille officiellement l'utilisation de GWMultiLaunch**.

La [Foire Aux Questions (FAQ) officielle de GWToolbox++](https://www.gwtoolbox.com/faq) indique clairement :

> **GWMultiLaunch n'est pas supporté et peut rencontrer des problèmes. GW Launcher est recommandé à la place.**

Elle mentionne également que l'utilisation de plusieurs programmes interagissant avec Guild Wars (comme Toolbox, des multi-lanceurs, des logiciels d'enregistrement, etc.) peut entraîner des plantages ou des comportements inattendus.

### 💡 Explication possible de votre problème

Même si les utilisateurs concernés ne lançaient pas *activement* GWToolbox++ au moment du problème, l'incompatibilité peut quand même se manifester :

1.  **Conflit de bas niveau :** GWToolbox++ et GWMultiLaunch cherchent tous deux à "s'accrocher" (hook) au client Guild Wars pour fonctionner. Même si Toolbox n'est pas visiblement lancé, il est possible que des composants (comme des fichiers .dll) ou des configurations résiduelles de Toolbox interfèrent avec la manière dont GWMultiLaunch gère les différentes instances du jeu.
2.  **Gestion des fenêtres :** Le blocage du Alt+Tab et les soucis de clavier suggèrent un conflit dans la gestion de la "priorité" (focus) des fenêtres et la capture des entrées (clavier/souris). C'est précisément le genre de choses que ces deux applications manipulent.
3.  **Recommandation d'alternative :** Le fait que l'équipe de Toolbox recommande spécifiquement "GW Launcher" (une alternative à GWMultiLaunch) renforce l'idée qu'il existe un conflit technique connu et non résolu avec GWMultiLaunch.

-----

### 🛠️ Pistes de solution

Voici les solutions et pistes de réflexion qui ressortent des recherches :

  * **Changer de Multi-Launcher :** La solution la plus évidente, recommandée par l'équipe de GWToolbox++, est de **migrer de GWMultiLaunch vers [GW Launcher](https://www.google.com/search?q=https://github.com/dane-light/gw-launcher)** (parfois appelé "dane-light's launcher"). Ce dernier semble être le standard actuel de la communauté pour le multi-boxing et est conçu pour être compatible avec Toolbox.
  * **Vérifier les "Overlays" :** Des problèmes d'Alt+Tab et de clavier dans Guild Wars sont aussi fréquemment causés par des superpositions (overlays) d'autres applications. Le plus souvent cité est **Discord**. Il est conseillé de désactiver l'overlay Discord (ou Nvidia, Steam, etc.) pour voir si cela résout le problème.
  * **Paramètres Windows :** Des réglages Windows comme la "Game Bar" (Barre de jeu) ou les "Optimisations du mode plein écran" peuvent parfois interférer avec la gestion des fenêtres de jeux plus anciens. Tenter de les désactiver pour l'exécutable `Gw.exe` peut aider.

En résumé, le problème que vous décrivez est très probablement le symptôme d'une **incompatibilité connue entre GWMultiLaunch et GWToolbox++**, même si ce dernier n'est pas actif. La solution la plus pérenne serait de tester le remplacement de GWMultiLaunch par GW Launcher.

J'espère que ces informations vous seront utiles pour dépanner les personnes concernées \!
