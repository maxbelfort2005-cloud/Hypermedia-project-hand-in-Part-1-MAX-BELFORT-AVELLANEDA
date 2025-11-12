# Hypermedia-project-hand-in-Part-1-MAX-BELFORT-AVELLANEDA
# Projecte: Curr铆culum Personal (Max Belfort Avellaneda)

Aquest repositori cont茅 el codi font d'un currículum web d'una sola pàgina, creat com a projecte. A continuació es detalla l'anàlisi del projecte tal com es demana a la documentació.

## 馃敆 Enlla莽os del Projecte

* **Lloc web publicat (GitHub Pages):** [https://your-username.github.io/your-repo-name/](https://your-username.github.io/your-repo-name/)
* **Projecte a Figma:** [Enlla莽 al teu projecte de Figma aqu铆](https://www.figma.com/...)

---

## 馃搫 Documentaci贸

### 1. An脿lisi del Projecte: Perfil d'Usuari (User Persona)

Per a aquest projecte, el "producte" 茅s el curr铆culum de Max Belfort Avellaneda, i els "usuaris" s贸n les persones que el llegiran. La *user persona* principal 茅s un reclutador o responsable de contractaci贸.

**Nom de la Persona:** Laura Mart铆n

* **Demografia:** 32 anys, viu a l'脿rea de Barcelona.
* **Rol:** Recrutadora t猫cnica a una petita o mitjana empresa de tecnologia o un estudi de desenvolupament de videojocs.
* **Objectius:** Trobar r脿pidament candidats adequats per a pr脿ctiques o posicions de nivell j煤nior (junior). Necessita avaluar l'adequaci贸 d'un candidat en menys d'un minut.
* **Necessitats:**
    * Veure clarament les dades de contacte.
    * Identificar r脿pidament la formaci贸 acad猫mica actual (Grau en Videojocs).
    * Escanejar qualsevol experi猫ncia laboral per avaluar la responsabilitat.
    * Identificar habilitats t猫cniques clau (Blender, SolidWorks, idiomes).
* **Punts de Dolor (Frustracions):**
    * CVs desordenats on no troba la informaci贸 que busca.
    * Llocs web que triguen a carregar o que no es veuen b茅 al m貌bil (sovint revisa perfils r脿pidament des del tel猫fon).
    * Formats massa "creatius" que amaguen la informaci贸 essencial.

**Com el disseny s'adre莽a a aquesta persona:**
El lloc web est脿 dissenyat per a la Laura. 脡s net, professional i va al gra. L'arquitectura lineal li permet escanejar de dalt a baix, trobant la informaci贸 en l'ordre que espera (Personal > Experi猫ncia > Formaci贸 > Habilitats).

---

### 2. An脿lisi del Projecte: Arquitectura de la Informaci贸

L'arquitectura de la informaci贸 (AI) d'aquest lloc web s'ha dissenyat seguint un **model lineal d'una sola p脿gina**. Aquesta decisi贸 茅s deliberada i es fonamenta en l'expectativa de l'usuari (el reclutador) quan consulta un curr铆culum vitae. L'objectiu principal 茅s la claredat, la rapidesa d'escaneig i l'accessibilitat, emulant la familiaritat d'un document de paper tradicional per貌 amb els avantatges del format web.

La informaci贸 s'ha estructurat de manera jer脿rquica i de dalt a baix, seguint un flux l貌gic que guia l'usuari a trav茅s del perfil del candidat. La p脿gina comen莽a amb un `<header>` clar que estableix el prop貌sit del lloc: "Curr铆culum".

Immediatament despr茅s, la primera `<section>` 茅s "Dades personals". Aquesta 茅s la informaci贸 m茅s cr铆tica per a un reclutador que vol contactar amb el candidat. S'ha organitzat com una llista (`<ul>`) perqu猫 s贸n elements de dades discrets i f脿cils d'escanejar.

A continuaci贸, s'ha prioritzat l'"Experi猫ncia professional". Tot i que la formaci贸 茅s important, molts reclutadors valoren l'experi猫ncia pr脿ctica, per modesta que sigui, ja que demostra responsabilitat i habilitats interpersonals. S'utilitza un element `<p>` perqu猫 茅s una descripci贸 narrativa.

Seguidament, la "Formaci贸 acad猫mica" detalla la traject貌ria educativa, crucial per a un perfil d'estudiant. De nou, s'utilitza una llista (`<ul>`) per a una clara separaci贸 dels diferents centres i etapes.

Finalment, la informaci贸 es tanca amb dues seccions d'habilitats: "Idiomes" i "Inform脿tica i altres". Aquestes seccions agrupen les compet猫ncies secund脿ries per貌 valuoses. Sem脿nticament, l'煤s d'etiquetes `<section>` per a cada bloc de contingut i t铆tols `<h2>` per a cada encap莽alament no nom茅s organitza visualment la p脿gina, sin贸 que tamb茅 la fa totalment accessible per a lectors de pantalla i millora la indexaci贸.

Aquesta arquitectura simple, sense navegaci贸 complexa ni enlla莽os interns, assegura que l'usuari consumeixi tota la informaci贸 presentada sense distraccions, complint l'objectiu de presentar un perfil professional de manera eficient.

---

### 3. An脿lisi del Projecte: Disseny Visual

El disseny visual del projecte s'ha centrat en el **minimalisme, la llegibilitat i el professionalisme**, amb un toc distintiu de color per crear una identitat visual memorable. L'objectiu 茅s transmetre serietat i claredat, evitant qualsevol distracci贸 visual.

**Paleta de Colors:**
La paleta 茅s deliberadament limitada. Es basa en un fons neutre, un gris molt clar (`#f7f9fc`), que 茅s m茅s suau per a la vista que el blanc pur. El text principal 茅s un gris fosc (`#222`), que proporciona un alt contrast per a la llegibilitat sense la duresa del negre pur (`#000`).
La identitat visual la proporcionen dos tons de verd:
1.  Un verd corporatiu, fosc i ser猫 (`#1f8855`), s'utilitza al `header` per crear un fort impacte inicial.
2.  Un verd ne贸 brillant (`#1fe13f`) s'utilitza per als t铆tols `<h2>`, actuant com a color d'accentuaci贸 que crida l'atenci贸 i guia l'usuari a les diferents seccions. Aquest toc de color vibrant sobre un disseny formal suggereix dinamisme i una connexi贸 amb sectors moderns (com el tecnol貌gic o el de videojocs).

**Tipografia:**
S'ha escollit una pila de fonts *sans-serif* (`"Segoe UI", Roboto, Helvetica, Arial, sans-serif`). Aquestes fonts s贸n conegudes per la seva excel路lent llegibilitat en pantalla, tant en dispositius d'escriptori com m貌bils. L'abs猫ncia de serifs d贸na un aspecte modern, net i t猫cnic, adequat per a un curr铆culum tecnol貌gic. La jerarquia tipogr脿fica 茅s clara: un `<h1>` gran al `header`, `<h2>` per a seccions, i un text de cos c貌mode amb un `line-height` d'1.6 per a una lectura f脿cil.

**Maquetaci贸 i Espaiat:**
La decisi贸 de disseny m茅s important 茅s el `max-width: 800px` i `margin: 0 auto`. Aix貌 centra el contingut i evita que el text s'estengui per tota la pantalla en monitors grans, la qual cosa 茅s una pr脿ctica fonamental per a la llegibilitat web.
S'ha fet un 煤s extensiu de l'espai en blanc (padding i margin) per "deixar respirar" el contingut. Visualment, el contingut principal (par脿grafs i elements de llista) es presenta en "targetes" blanques (`background-color: #fff`) amb una vora subtil i una ombra (`box-shadow`). Aquest efecte "eleva" el contingut del fons gris, creant profunditat i organitzant clarament els blocs d'informaci贸.

**Disseny Responsive:**
S'ha incl貌s una *media query* b脿sica (`@media (max-width: 600px)`). En dispositius m貌bils, es redueix el padding i la mida de les fonts per optimitzar l'espai disponible, garantint que el curr铆culum sigui perfectament funcional i llegible en qualsevol pantalla.
