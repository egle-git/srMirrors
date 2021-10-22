# Specialaus reliatyvumo judėjimo vaizdavimas - erdvėlaikio diagramos

Kalbėdamas apie apie šviesos greičio pastovumą inertinėse atskaitos sistemose
D.Hogg aptaria du stebėtojus, Deepto (D) ir Eriką (E), kurie juda vienas kito
atžvilgiu, rankoje laikydami šviesos laikrodį.

<img src="Doc/Hogg-fig-2p1.png" alt="" />

<img src="Doc/Hogg-fig-2p2.jpg" alt="" />

<br>

Kai bandome šviesos judėjimą pavaizduoti erdvėlaikio diagramose, vaizdas gali
pasidaryti gana painus.

<img src="Doc/Hogg-fig-3p11.png" alt="" />

<br>

Ypač, kai vaizduojamas šviesos judėjimas tarp veidrodžių, pačių veidrodžių
nerodant

<img src="Doc/TGajdosik-spacetime-diagram.png" alt="" />


Bandydamas suprasti, kaip atrodo šviesos judėjimas 3D diagramoje, buitiškai
pasirašiau programėlę panaudodamas ROOT bibliotekas.

Pirminis, prototipinis kodas - `drawMirror.C` - vėliau virto kiek pažangesniu
kodu `drawMirror2.C`. Kodai leidžia pavaizduoti šviesos judėjimą laikrodžiuose,
vaizduojant stovintį stebėtoją ir judančio stebėtoją atskirai. Nebandžiau
suderinti stebėtojų laikrodžių - man norėjosi pamatyti kokiu būdu nepilname
vaizdavime gali susidaryti įspūdis, kad šviesa juda $x$ kryptimi pirmyn-atgal.

ROOT macro `drawMirror2` turi tris argumentus: laiko indeksą (`time_pos`), ar 
reikia piešinėlius išsaugoti (`doSave`) ir ar laikrodis juda (`move`).

Iš pradžių tiesiog norėjau išsaugoti piešinėlius, tai pasirašiau `bash`
skriptą `run2.sh`, o paskui supratau, kad galiu pagaminti ir animacinį `gif`
paveikslėlį, tad parašiau `anim.sh`.

Sėkmės išbandant.


<br>
**Bibliography**

[1] D.W.Hogg, "Special Relativity", Lecture notes, December 1, 1997.
