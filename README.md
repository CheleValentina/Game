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
