========================INSTRUCTIUNI========================

Noaptea trecuta a avut loc un jaf la o importanta banca din Cluj-Napoca. Ai fost desemnat principalul detectiv pentru a prinde vinovatul. Cloneaza acest repository, urmeaza indiciile si rezolva misterul!

1. Creeaza un branch nou cu numele tau. Acesta va fi principalul loc unde iti vei desfasura investigatia. Muta-te pe branch.

2. Creeaza un fisier nou cu denumirea "NUMELE_TAU_investigatie.txt" si scrie numele tau in el. Vei avea nevoie de fisier mai tarziu, asa ca adauga-l in staging area, apoi fa commit pentru a-l publica in repository-ul local.

3. Publica branch-ul pentru a ii tine la curent si pe ceilalti detectivi legat de investigatia ta. Dupa ce ai publicat branch-ul, fa merge la branch-ul "suspects" in branch-ul tau si urmeaza noile instructiuni.

---------------------------COMENZI--------------------------

git clone <ssh_url>

git branch <nume_branch>

git checkout <nume_branch>

git add <nume_fisier>

git commit -m "Mesaj de commit"

git push --set-upstream origin <nume_branch>

git merge suspects

============================================================
=======================INSTRUCTIUNI 2=======================

Felicitari! Ai primit lista de suspecti in fisierul "suspects.txt".

Publica modificarile din branch-ul tau cu "git push", pentru a-i informa si pe ceilalti detectivi.

Pentru a continua investigatia, fa merge la branch-ul "hint1" in branch-ul tau.

---------------------------COMENZI--------------------------

git push

git merge hint1

============================================================
=======================INSTRUCTIUNI 3=======================

Vesti bune! In urma unor investigatii, o parte dintre suspecti au fost eliminati din lista de suspecti.

Verifica sa vezi care suspecti au fost eliminati cu "git diff <id_commit_anterior> suspects.txt". 

Deschide fisierul creat de tine la pasul anterior cu investigatia ta, scrie "Nu sunt suspecti:" in fisier, apoi adauga numele suspectilor care au fost eliminati (foloseste copy-paste). Adauga fisierul tau in staging area, apoi fa commit la modificari.

Publica modificarile pentru a-i informa si pe ceilalti detectivi.

Pentru a continua investigatia, fa merge la branch-ul "hint2" in branch-ul tau.

---------------------------COMENZI--------------------------

git diff <commit_id> suspects.txt

git add <nume_fisier>

git commit -m "Mesaj de commit"

git push

git merge hint2

============================================================
=======================INSTRUCTIUNI 4=======================

Oops! Cativa suspecti au fost stersi din greseala! Fa revert la ultimele 3 commit-uri care au denumirea "Remove suspects" pentru a primi inapoi suspectii.

Publica modificarile, apoi fa merge la branch-ul "hint3" in branch-ul tau pentru a continua investigatia.

---------------------------COMENZI--------------------------

git log

git revert <commit_id>

git push

git merge hint3

============================================================
=======================INSTRUCTIUNI 5=======================

Au mai ramas doar 3 suspecti. Pentru a primi informatii importante, fa merge la branch-ul "hint4" in branch-ul tau, apoi fa merge la branch-ul "hint5" in branch-ul tau. Atentie! Va trebui sa rezolvi un conflict.

Dupa ce rezolvi conflictul, urmeaza instructiunea primita in "instruction.txt", adauga fisierele "instruction.txt" si fisierul "suspects.txt" in staging area, fa commit, publica modificarile, apoi fa merge la branch-ul "hint6" pentru a continua investigatia.

---------------------------COMENZI--------------------------

git merge hint4

git merge hint5

git add <nume_fisier>

git commit -m "Mesaj de commit"

git push

git merge hint6

============================================================
=======================INSTRUCTIUNI 6=======================

Vesti bune! A existat o scurgere de informatii si numele unui suspect a fost afisat din greseala!

Acest lucru s-a intamplat pe branch-ul "hint7". Pentru a obtine informatia, muta-te pe branch-ul hint7, copiaza id-ul commit-ului cu numele "Remove unnecessary suspects", muta-te inapoi pe branch-ul tau si foloseste "git cherry-pick" pentru a copia commit-ul.

Publica modificarile, apoi fa merge la branch-ul "hint8" in branch-ul tau.

---------------------------COMENZI--------------------------

git checkout hint7

git checkout <your_branch>

git cherry_pick <commit_id>

git push

git merge hint8

============================================================
============================FINAL===========================

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
FELICITARI! AI GASIT VINOVATUL! Publica modificarile, apoi fa un pull request pentru a incheia jocul.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

============================================================
