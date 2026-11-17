# BFK LAB – Anatomie și Kinetoterapie

Versiunea demonstrativă 1.0 a unei aplicații web educaționale în limba română.

## Ce include
- cinci module introductive: Oase, Mușchi, Articulații, Planuri și axe, Kinetoterapie;
- lecții scurte și structură modulară;
- câte un test cu feedback explicativ pentru fiecare modul;
- design adaptiv pentru telefon, tabletă și laptop;
- instalare ca PWA atunci când aplicația este publicată prin HTTPS;
- funcționare offline după prima încărcare (în browsere compatibile).

## Testare locală
Deschideți `index.html` într-un browser pentru o previzualizare. Pentru testarea completă a instalării PWA și a modului offline, serviți folderul printr-un server local sau publicați-l prin HTTPS.

## Publicare gratuită (variantă simplă)
1. Creați un cont pe GitHub și un repository nou, de exemplu `bfk-lab`.
2. Încărcați toate fișierele din acest folder în repository.
3. În repository, accesați Settings → Pages.
4. La Build and deployment selectați Deploy from a branch, apoi `main` și `/ (root)`.
5. Salvați. GitHub va genera o adresă publică de forma `https://utilizator.github.io/bfk-lab/`.
6. Distribuiți linkul colegilor. Pe telefoanele compatibile, browserul poate oferi opțiunea de instalare/adăugare pe ecranul principal.

Interfața GitHub se poate modifica; dacă pașii diferă, consultați documentația GitHub Pages.

## Cum se dezvoltă
Conținutul este păstrat în lista `modules` din `app.js`. Fiecare modul are:
- `id`, `n`, `icon`, `title`, `desc`, `intro`;
- `sections`: titlu și text pentru fiecare subcapitol;
- `fact`: casetă de recapitulare;
- `quiz`: întrebare, variante, indexul răspunsului corect și explicație.

Pentru o dezvoltare mai amplă, se recomandă separarea conținutului în fișiere JSON, adăugarea unui atlas anatomic cu imagini licențiate, teste cu mai multe întrebări, conturi și sincronizarea progresului printr-un backend. Nu introduceți date personale sau medicale ale pacienților în această versiune.

## Limitări importante
Aceasta este o versiune MVP educațională, nu o platformă clinică și nu un produs medical. Conținutul este introductiv și trebuie verificat editorial de cadre didactice/specialiști înainte de utilizare ca material didactic oficial. Nu include încă atlas 3D, autentificare, baze de date, panou de administrare sau încărcare de cursuri de către utilizatori.
