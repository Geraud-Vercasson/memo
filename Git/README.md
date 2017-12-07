Liste des commandes git

init : 
Cr�e un dossier git vide, ou (r�)initialise un dossier d�j� existant

status :
R�cup�re l'�tat actuel du dossier git

add : 
Ajoute le(s) �l�ment(s) dans la liste des fichiers et dossiers � g�rer par git

commit : 
Enregistre et nomme (via -m "") les changements effectu�s

log :
Affiche  tous les changements enregistr�s (les commit)

remote add origin:
Ajoute au dossier git un "repository" distant, et le lie a udossier 'origin'

push :
envoie sur le repo distant les modifications enregistr�es dans le dernier commit.

push -u origin master:
-u permet de se rappeler, das ce contexte d'utilisation, quels sont les param�tres de la fonction push :
	origin : l'�l�ment � push (notre repo local)
	master : le nom de la 'branch' dans laquelle nous allons push notre �l�ment

pull :
r�cup�re les changements du repo distant sur notre repo local

pull origin master:
'pull' dans origin ce qui vient de master

diff:
Montre les diff�rences entre l'�tat actuel de notre repo local et un �tat 'committ�'

diff HEAD:
Pr�cise que l'�tat auquel on veut comparer est le dernier commit

diff --staged:
??

reset :
inverse de add sur un �l�ment. Si c'est un �l�ment qui a �t� 'add' au pr�sent commit, il ne le sera plus.

checkout :
remet l'�l�ment � l'�tat du pr�c�dent commit

branch <NewBranchName>:
cr�e une "branch" sur notre "arbre". On cr�e ainsi un nouveau contexte, ind�pendant de la branch "master", dans lequel nous allons travailler. on poura les merge �ventuellement plus tard

branch:
Liste l'ensemble des branch actuellement disponibles.

checkout <BranchName>:
change de "branch" de travail, on travaille d�sormais sur la branch <BranchName>

rm <>:
remove -> supprime de notre repo local le(s) �l�ment(s) <>, et notifie git de cette suppression (ajout dans le journal)

merge <BranchToMerge>:
fusionne la branch dans laquelle on travaille avec la branch <BranchToMerge>

branch -d <BranchToDelete>:
supprime la branch <BranchToDelete>

