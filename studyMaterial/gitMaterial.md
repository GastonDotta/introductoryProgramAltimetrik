Git: ![img](https://lh3.googleusercontent.com/dnyDO-4zLMWbPGdEz7kMS1wtrTuzvEpNjWCswck1WAT9ADcoJHkxfB9I09hfUh69lv2VPggt3tbqLj_HaxjAWGvtP7yIj0Y0U2GmyaQ2BRRQdNklrWnFx27ZXNdJn-4-svnyZmID)Git es el[ Version Control System](https://www.atlassian.com/es/git/tutorials/what-is-version-control) de código abierto más popular del mercado.

### Branches:

Cuando se crea el primer "Commit" automáticamente se crea la rama "Master", es que <u>en Git se suelen utilizar los sistemas de ramificaciones para que si se debe arreglar un "bug" o agregar una nueva funcionalidad simplemente se pueda seguir trabajando en el "Master" permitiendo así realizar mantenimientos o cambios a las demás ramas sin necesidad de alterar el esqueleto.</u>

### Branching Strategies & Flows: 

Como se detalló se utilizan distintas branches para trabajar de formas distintas y un equipo de desarrollo siempre debería de trazarse una estrategia de branches. [Este Flowchart suele ser el más utilizado](https://nvie.com/img/git-model@2x.png) (Gitflow) <u>suele ser de las más comunes y propone la división con 2 tipos de branches esenciales la branch “Master”, y la rama “Develop”, a la cual se le pueden sumar las “Feature” branches, “Release” branches y “Hotfix” branches.</u>

La branch Master suele contener las “Versiones” por lo cual se le suelen hacer muy pocos cambios y se trabaja más que nada en la rama “Develop” en la cual una vez que los cambios realizados son “estables” y chequeados se hace un “merge” a una nueva versión en Master.

Por otro lado las *“Feature branches” como indica la palabra se utilizan para desarrollar nuevas características del programa*, una vez terminada se “mergea” en la rama develop y pasa a abrirse la *“Release Branch” donde se “testea” la función, se arreglan “bugs” y se trabaja la metadata para lanzar*(release) una nueva versión en futuro. 

Las *“Hotfix Branches”* son las que nadie quiere tener, es una rama que se desprende directamente del “Master” y *suele utilizarse para arreglar “bugs” severos.*

### Tags and commits:

<u>Los commits son como pequeñas "capturas de pantalla" del proyecto</u> que se está trabajando estos son muy livianos, y cambiar de uno a otro es terriblemente rápido. Git pretende mantener los commits tan livianos como sea posible, por lo que no copia ciegamente el directorio completo cada vez que se hace un commit. Puede (cuando es posible) comprimir un commit como un conjunto de cambios entre una versión del repositorio y la siguiente.A el primer commit se le llama "Head" y siempre los nuevos son hijos directos del último commit. 

<u>En Git se puede "etiquetar" puntos específicos</u> de la historia de un repositorio, esto por lo general se utiliza para marcar cambios en la funcionalidad, estética o versión (v1.0, v1.1, etc.) pero también se puede utilizar un mensaje en la misma para internamente saber cuales son los cambios que esta "captura de pantalla" contiene.

Ej. *git-commit -a "tag" -m "cambios de la tag"*

### Stash command:

‘’Stash’’ proviene de la palabra cofre o alijo, este comando *crea una ‘’caja’’ donde se guardan los cambios realizados sin commitear* para poder salir de la rama trabajar en otra y que cuando se quiera se pueda acceder a esos cambios en esa ‘’caja’' en donde quiera que esté.

### Hooks:

Son mecanismos que activan <u>scripts estos están destinados a automatizar acciones dentro de git.</u>

Los Hooks se almacenan en la carpeta .git/hooks/ de cada proyecto clonado, o en un repositorio local recién creado. [Allí encontraremos una serie de hooks de ejemplo](https://www.hostinger.es/tutoriales/como-usar-git-hooks).

### Rebase and squash: 

<u>La reorganización (Rebase) es el proceso de mover o combinar una secuencia de commits en una nueva commit base.</u> La reorganización suele ser muy útil y se visualiza fácilmente en el contexto de un flujo de trabajo de ramas de funciones.

<u>Squash se refiere a reunir varios commit en uno solo (de una misma branch).</u>

### Merge vs rebase:

<u>El rebase unifica las ramas dejando un arbol lineal ‘’dejandoló más prolijo’’. El merge aun deja ‘’vivo’’ el gráfico de las ramas.</u>
El rebase unifica las ramas perdiendo el historial de los commit y el merge no. 

Esto puede resultar muy importante cuando se necesite llevar o saber el historial de commit y se esta trabajando con otros compañeros en esa rama.



### Bibliografía: 



[Git Tutorial for Beginners: Learn Git in 1 Hour - Programming with Mosh](https://www.youtube.com/watch?v=8JJ101D3knE)

[Git About - Git-scm](https://git-scm.com/about)

[Git Tags - Git-Scm](https://git-scm.com/book/en/v2/Git-Basics-Tagging)

[Git Commit - Git-scm](https://git-scm.com/docs/git-commit)

[Choose the right Git branching strategy](https://www.creativebloq.com/web-design/choose-right-git-branching-strategy-121518344)

[A successful Git branching model » nvie.com](https://nvie.com/posts/a-successful-git-branching-model/)

[Flujo de trabajo de Gitflow](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

[DIFERENCIA ENTRE GIT REBASE Y GIT MERGE , WORKSHOP DE GIT .](https://medium.com/@MiguelCasas/diferencia-entre-git-rebase-y-git-merge-workshop-de-git-8622dedde2d7)

[How to Squash Commits in Git | Learn Version Control with Git](https://www.git-tower.com/learn/git/faq/git-squash/)

[Git MERGE vs REBASE](https://www.youtube.com/watch?v=CRlGDDprdOQ&ab_channel=ProgrammingwithMoshProgrammingwithMoshVerificada) 

[git-stash Documentation](https://git-scm.com/docs/git-stash)

[El comando Stash para cambios rápidos en un proyecto en Git](https://www.runroom.com/realworld/git-stash)

[What is the intended use-case for git stash?](https://stackoverflow.com/questions/20537223/what-is-the-intended-use-case-for-git-stash) 

