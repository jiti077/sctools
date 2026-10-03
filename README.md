#SC TOOLS
Eina avançada de gràfics científics amb desviació estàndard
SC TOOLS és una aplicació web de codi obert per crear, editar i exportar gràfics científics de barres amb mitjana ± desviació estàndard (SD).
Està pensada especialment per a treballs de recerca, laboratoris, projectes acadèmics, figures científiques i presentacions de resultats.

L'aplicació funciona 100 % al navegador i de manera local, sense necessitat de servidor ni base de dades.

✨ Característiques principals
📊 Creació de gràfics de barres científics.
📐 Representació de valors amb ± desviació estàndard (SD).
✏️ Edició interactiva de categories, valors i desviacions.
🎨 Colors personalitzables per a cada barra.
🖌️ Diverses paletes de colors predefinides:
Blau Office
Excel Clàssic
Científica
Monocromàtica / escala de grisos
📏 Configuració manual o automàtica de l'escala de l'eix Y.
🔢 Configuració personalitzada dels ticks de l'eix Y.
📋 Possibilitat de crear diversos gràfics dins d'un mateix projecte.
📑 Duplicació i eliminació de gràfics.
🧩 Creació de matrius de gràfics.
🔲 Diferents distribucions de matriu:
1 × 1
1 × 2
2 × 2
2 × 3
3 × 1
3 × 3
2 × 4
4 × 2
📝 Títol i subtítol generals per a les figures.
⚙️ Configuració de les barres d'error.
📐 Ajust de l'amplada dels caps de les barres d'error.
📏 Ajust del gruix de les línies d'error.
➕ Representació de +SD o ±SD.
📊 Activació/desactivació de línies de retícula.
🔢 Visualització opcional dels valors sobre les barres.
🖼️ Exportació de gràfics en format PNG.
🚀 Exportació en diferents resolucions:
Estàndard
HD (2×)
Ultra HD / impressió (3×)
💾 Desament dels projectes en format JSON.
📂 Carregament de projectes JSON.
🧪 Dades d'exemple per provar l'aplicació.
🌐 Interfície completament en català.
🚀 Com utilitzar SC TOOLS
No cal instal·lar cap dependència ni configurar cap servidor.
1. Obrir l'aplicació
Descarrega o clona el repositori i obre el fitxer:
index.html

directament amb un navegador web modern.
També es pot publicar fàcilment com a pàgina web estàtica.

2. Crear un gràfic
En iniciar l'aplicació es crea automàticament un gràfic inicial.
Des de 1. Gràfics i Dades pots modificar:

Títol del gràfic
Etiqueta de l'eix X
Etiqueta de l'eix Y
Escala de l'eix Y
Categories
Valors
Desviacions estàndard
Colors de les barres
Per afegir una nova barra, prem:
Afegir Barra

📊 Desviació estàndard
Cada barra pot tenir associada una desviació estàndard:
Valor = 5.0
SD    = 0.5

El gràfic mostrarà:
5.0 ± 0.5

Les barres d'error es poden personalitzar des de:
2. Estil i Desviació (SD)

Es poden modificar:

Amplada del cap de la barra d'error
Gruix de la línia
Color
Representació ±SD
Representació només de +SD
🎨 Paletes de colors
SC TOOLS incorpora quatre paletes predefinides.
Blau Office
Inspirada en la paleta habitual de Microsoft Office/Excel.
Excel Clàssic
Una paleta de colors més fosca i contrastada.
Científica
Una paleta pensada per a figures científiques, amb colors diferenciats i contrastats.
Monocromàtica
Escala de grisos adequada per a figures en blanc i negre o publicacions que requereixin una representació monocromàtica.
També es pot seleccionar manualment el color de cada barra.

🧩 Matrius de gràfics
L'aplicació permet combinar diversos gràfics en una única figura.
Des de:

3. Matriu Agrupada

es pot seleccionar una distribució de gràfics i assignar cada gràfic a una posició concreta.

Per exemple:

┌─────────────┬─────────────┐
│   Gràfic A  │   Gràfic B  │
├─────────────┼─────────────┤
│   Gràfic C  │   Gràfic D  │
└─────────────┴─────────────┘

També es pot definir:
Títol general de la figura
Subtítol
Assignació dels gràfics
Distribució de la matriu
Aquesta funcionalitat és especialment útil per crear figures compostes per a informes, treballs acadèmics o publicacions.
💾 Desar i carregar projectes
Els projectes es poden desar en format .json.
Des del menú:

Fitxer → Desar Projecte

es genera un fitxer amb tot l'estat de l'aplicació.

Posteriorment es pot recuperar amb:

Fitxer → Obrir Projecte

Això permet guardar el treball i continuar-lo posteriorment sense necessitat de cap servidor.

Exemple
Projecte_SCTOOLS_1720000000000.json

El fitxer JSON conté:
Gràfics
Dades
Colors
Configuració dels eixos
Configuració de les barres d'error
Configuració visual
Configuració de la matriu
🖼️ Exportació
Els gràfics es poden exportar directament en format:
PNG

Hi ha tres nivells de resolució:
Resolució	Escala
Estàndard	1×
HD	2×
Impressió / Ultra HD	3×

La renderització es realitza mitjançant un element HTML <canvas>.
Això permet generar imatges d'alta resolució sense necessitat d'utilitzar un servidor extern.

🧪 Dades d'exemple
L'aplicació inclou un botó:
Carregar Exemple

que permet carregar dades de demostració.

Aquest exemple inclou diversos gràfics amb dades simulades de laboratori, incloent:

Assaig enzimàtic
Expressió genètica
Valors mitjans
Desviacions estàndard
És útil per comprovar ràpidament les funcionalitats de l'aplicació.
🛠️ Tecnologies
SC TOOLS està desenvolupat com una aplicació web client-side.
Tecnologies principals
HTML5
JavaScript
CSS
HTML Canvas
Tailwind CSS
Font Awesome
Google Fonts — Inter
No utilitza:
Backend
Base de dades
API pròpia
Sistema d'autenticació
Servidor d'aplicació
El projecte funciona principalment al navegador.
📁 Estructura recomanada del projecte
Una estructura senzilla per publicar-lo a GitHub és:
SC-TOOLS/
│
├── index.html
├── README.md
└── LICENSE

Actualment, la major part de l'aplicació es troba continguda dins de index.html.
En futures versions, el projecte es podria separar en:

SC-TOOLS/
│
├── index.html
├── css/
│   └── styles.css
├── js/
│   ├── app.js
│   ├── charts.js
│   ├── export.js
│   └── state.js
├── README.md
└── LICENSE

🌐 Publicació amb GitHub Pages
SC TOOLS es pot publicar com una pàgina web estàtica.
Una opció és utilitzar GitHub Pages.

Passos generals:

Crea un repositori a GitHub.
Puja index.html.
Puja aquest README.md.
Ves a la configuració del repositori.
Activa GitHub Pages.
Selecciona la branca que conté els fitxers del projecte.
GitHub generarà una URL pública per a l'aplicació.
No cal configurar cap backend.
🔒 Privacitat
SC TOOLS està dissenyat per funcionar localment al navegador.
Les dades introduïdes als gràfics no necessiten ser enviades a cap servidor de SC TOOLS.

Els projectes es poden exportar manualment a fitxers JSON i gestionar-los localment.

Nota: l'aplicació utilitza recursos externs per carregar Tailwind CSS, Font Awesome i la font Inter. Per tant, el navegador pot requerir connexió a Internet per carregar aquests recursos si no s'han incorporat localment al projecte.
📜 Llicència
SC TOOLS es distribueix sota la llicència MIT.
Això permet, entre altres coses:

Utilitzar el projecte.
Copiar-lo.
Modificar-lo.
Distribuir-lo.
Utilitzar-lo en projectes personals o comercials.
Consulta el fitxer LICENSE del repositori per veure el text complet de la llicència.
🤝 Contribucions
Les contribucions són benvingudes.
Si vols millorar SC TOOLS, pots:

Fer un fork del repositori.
Crear una branca per al canvi.
Implementar la millora o correcció.
Fer un commit amb els canvis.
Obrir un Pull Request.
També pots obrir una Issue per informar d'errors, proposar funcionalitats o comentar possibles millores.
💡 Possibles millores futures
Algunes funcionalitats que es podrien incorporar en versions futures:
Exportació SVG.
Exportació PDF.
Importació de dades CSV.
Copiar i enganxar dades directament des d'Excel.
Més tipus de gràfics.
Gràfics de dispersió.
Boxplots.
Gràfics de línies.
Intervals de confiança.
Error estàndard (SEM).
Intervals personalitzats.
Edició de tipografies.
Més opcions d'exportació.
Sistema de plantilles.
Suport per a figures de publicació més avançades.
Separació del codi HTML, CSS i JavaScript.
📌 Estat del projecte
SC TOOLS v2.5
Projecte de codi obert orientat a la creació de figures científiques i acadèmiques.

L'aplicació està pensada com una eina lleugera, local i fàcil d'utilitzar per preparar gràfics amb desviació estàndard i figures compostes.

👨‍🔬 Filosofia del projecte
SC TOOLS busca oferir una alternativa senzilla i accessible per crear figures científiques sense necessitat d'utilitzar eines complexes.
La idea és mantenir un entorn de treball:

Simple
Local
Transparent
Reproduïble
Personalitzable
De codi obert
SC TOOLS — Eina de gràfics científics de codi obert
Llicència MIT · Funcionament local · v2.5
