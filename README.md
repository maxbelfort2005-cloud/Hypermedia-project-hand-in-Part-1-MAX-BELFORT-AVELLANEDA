# Projecte: Currículum Personal (Max Belfort Avellaneda)

Aquest repositori conté el codi font d'un currículum web d'una sola pàgina, creat com a projecte. A continuació es detalla l'anàlisi del projecte tal com es demana a la documentació.

## 🔗 Enllaços del Projecte

* **Projecte a Figma:** [Enllaç al teu projecte de Figma aquí](https://www.figma.com/design/T2Rvo7zUaNKJAtbzLN8QGo/El-equipo-de-Max-Belfort-team-library?node-id=0-1&t=JSG6AceoGVGEoyOu-1)

---

## 📄 Documentació

### 1. Anàlisi del Projecte: Perfil d'Usuari (User Persona)

Per a aquest projecte, el "producte" és el currículum de Max Belfort Avellaneda, i els "usuaris" són les persones que el llegiran. La *user persona* principal és un reclutador o responsable de contractació.

**Nom de la Persona:** Laura Martín

* **Demografia:** 32 anys, viu a l'àrea de Barcelona.
* **Rol:** Recrutadora tècnica a una petita o mitjana empresa de tecnologia o un estudi de desenvolupament de videojocs.
* **Objectius:** Trobar ràpidament candidats adequats per a pràctiques o posicions de nivell júnior (junior). Necessita avaluar l'adequació d'un candidat en menys d'un minut.
* **Necessitats:**
    * Veure clarament les dades de contacte.
    * Identificar ràpidament la formació acadèmica actual (Grau en Videojocs).
    * Escanejar qualsevol experiència laboral per avaluar la responsabilitat.
    * Identificar habilitats tècniques clau (Blender, SolidWorks, idiomes).
* **Punts de Dolor (Frustracions):**
    * CVs desordenats on no troba la informació que busca.
    * Llocs web que triguen a carregar o que no es veuen bé al mòbil (sovint revisa perfils ràpidament des del telèfon).
    * Formats massa "creatius" que amaguen la informació essencial.

**Com el disseny s'adreça a aquesta persona:**
El lloc web està dissenyat per a la Laura. És net, professional i va al gra. L'arquitectura lineal li permet escanejar de dalt a baix, trobant la informació en l'ordre que espera (Personal > Experiència > Formació > Habilitats).

---

### 2. Anàlisi del Projecte: Arquitectura de la Informació

L'arquitectura de la informació (AI) d'aquest lloc web s'ha dissenyat seguint un **model lineal d'una sola pàgina**. Aquesta decisió és deliberada i es fonamenta en l'expectativa de l'usuari (el reclutador) quan consulta un currículum vitae. L'objectiu principal és la claredat, la rapidesa d'escaneig i l'accessibilitat, emulant la familiaritat d'un document de paper tradicional però amb els avantatges del format web.

La informació s'ha estructurat de manera jeràrquica i de dalt a baix, seguint un flux lògic que guia l'usuari a través del perfil del candidat. La pàgina comença amb un `<header>` clar que estableix el propòsit del lloc: "Currículum".

Immediatament després, la primera `<section>` és "Dades personals". Aquesta és la informació més crítica per a un reclutador que vol contactar amb el candidat. S'ha organitzat com una llista (`<ul>`) perquè són elements de dades discrets i fàcils d'escanejar.

A continuació, s'ha prioritzat l'"Experiència professional". Tot i que la formació és important, molts reclutadors valoren l'experiència pràctica, per modesta que sigui, ja que demostra responsabilitat i habilitats interpersonals. S'utilitza un element `<p>` perquè és una descripció narrativa.

Seguidament, la "Formació acadèmica" detalla la trajectòria educativa, crucial per a un perfil d'estudiant. De nou, s'utilitza una llista (`<ul>`) per a una clara separació dels diferents centres i etapes.

Finalment, la informació es tanca amb dues seccions d'habilitats: "Idiomes" i "Informàtica i altres". Aquestes seccions agrupen les competències secundàries però valuoses. Semànticament, l'ús d'etiquetes `<section>` per a cada bloc de contingut i títols `<h2>` per a cada encapçalament no només organitza visualment la pàgina, sinó que també la fa totalment accessible per a lectors de pantalla i millora la indexació.

Aquesta arquitectura simple, sense navegació complexa ni enllaços interns, assegura que l'usuari consumeixi tota la informació presentada sense distraccions, complint l'objectiu de presentar un perfil professional de manera eficient.

---

### 3. Anàlisi del Projecte: Disseny Visual

El disseny visual del projecte s'ha centrat en el **minimalisme, la llegibilitat i el professionalisme**, amb un toc distintiu de color per crear una identitat visual memorable. L'objectiu és transmetre serietat i claredat, evitant qualsevol distracció visual.

**Paleta de Colors:**
La paleta és deliberadament limitada. Es basa en un fons neutre, un gris molt clar (`#f7f9fc`), que és més suau per a la vista que el blanc pur. El text principal és un gris fosc (`#222`), que proporciona un alt contrast per a la llegibilitat sense la duresa del negre pur (`#000`).
La identitat visual la proporcionen dos tons de verd:
1.  Un verd corporatiu, fosc i serè (`#1f8855`), s'utilitza al `header` per crear un fort impacte inicial.
2.  Un verd neó brillant (`#1fe13f`) s'utilitza per als títols `<h2>`, actuant com a color d'accentuació que crida l'atenció i guia l'usuari a les diferents seccions. Aquest toc de color vibrant sobre un disseny formal suggereix dinamisme i una connexió amb sectors moderns (com el tecnològic o el de videojocs).

**Tipografia:**
S'ha escollit una pila de fonts *sans-serif* (`"Segoe UI", Roboto, Helvetica, Arial, sans-serif`). Aquestes fonts són conegudes per la seva excel·lent llegibilitat en pantalla, tant en dispositius d'escriptori com mòbils. L'absència de serifs dóna un aspecte modern, net i tècnic, adequat per a un currículum tecnològic. La jerarquia tipogràfica és clara: un `<h1>` gran al `header`, `<h2>` per a seccions, i un text de cos còmode amb un `line-height` d'1.6 per a una lectura fàcil.

**Maquetació i Espaiat:**
La decisió de disseny més important és el `max-width: 800px` i `margin: 0 auto`. Això centra el contingut i evita que el text s'estengui per tota la pantalla en monitors grans, la qual cosa és una pràctica fonamental per a la llegibilitat web.
S'ha fet un ús extensiu de l'espai en blanc (padding i margin) per "deixar respirar" el contingut. Visualment, el contingut principal (paràgrafs i elements de llista) es presenta en "targetes" blanques (`background-color: #fff`) amb una vora subtil i una ombra (`box-shadow`). Aquest efecte "eleva" el contingut del fons gris, creant profunditat i organitzant clarament els blocs d'informació.

**Disseny Responsive:**
S'ha inclòs una *media query* bàsica (`@media (max-width: 600px)`). En dispositius mòbils, es redueix el padding i la mida de les fonts per optimitzar l'espai disponible, garantint que el currículum sigui perfectament funcional i llegible en qualsevol pantalla.
