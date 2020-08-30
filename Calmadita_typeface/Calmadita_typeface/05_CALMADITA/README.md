# Calmadita

## How to build fonts and sources

### Clone a repository
1. Create a folder on your computer to put your repository in
2. Go to Github and clink on the clone http button to copy the link
3. In Terminal or Command Line go to the repository typing:
cd "repository path", hit enter
4. Then type: git clone "paste here the link you copy from github", hit enter
5. Now you have a copy of all docuemnt on your computer and you are ready to work on it

### Activate the virtual enviroment
1. Before give any git command type: source venv.sh

### UFO to glyphs
To generate your .glyphs file based on .ufo sources (mixing uprights and italics)

ufo2glyphs sources/Calmadita.designspace 

### Glyphs to UFOs
To update .ufo sources from your .glyphs file

glyphs2ufo sources/Calmadita.glyphs

### Generate static fonts (otf or ttf)
Copy paste these 4 commands in the command line

fontmake -m sources/Calmadita.designspace -o ttf 
fontmake -m sources/Calmadita.designspace -o otf


### Generate variable fonts
fontmake -m sources/Calmadita.designspace -o variable

###Generate webfonts
pyftsubset Calmadita_Rg.ttf '*' --flavor='woff' --obfuscate-names


## Cómo crear tipografías y fuentes editables

### Clonar el repositorio
1. Crea una carpeta en tu computadora para colocar tu repositorio
2. Vae a Github y haz clic en el botón clonar http para copiar el enlace
3. En Terminal o Línea de comandos, ve al repositorio escribiendo:
cd "ruta del repositorio" 
Presiona enter
4. Luego escribe: git clone "pega aquí el enlace que copiaste de github"
Presiona enter
5. Ahora tienes una copia de todos los documentos en tu computadora y estás listx para trabajar en él.

### Activa el entorno virtual
1. Antes de dar cualquier tipo de comando git teclea:
source venv.sh

### UFO a Glyphs
Para generar tu archivo .glyphs basado en fuentes .ufo (uniendo redondas e italicas)

ufo2glyphs sources / Calmadita.designspace


### Glyphs a UFO
Para actualizar las fuentes .ufo de tu archivo .glyphs

glyphs2ufo sources / Calmadita.glyphs


### Genera fuentes estáticas (otf o ttf)
Copia y pega estos comandos en la línea de comandos (uno a la vez)

fontmake -m fuentes / Calmadita.designspace -o ttf
fontmake -m fuentes / Calmadita.designspace -o otf


### Genera fuentes variables
fontmake -m fuentes / Calmadita.designspace -o variable

### Generar fuentes web
pyftsubset Calmadita_Rg.ttf '*' --flavor = 'woff' --obfuscate-names


2020 Copyright

Fede Biagioli:  fjbiagioli@gmail.com
Iordan Evair: iordan_e@outlook.es
Leonardo Delgado: delgadotype@gmail.com
Jorge George: jorgejgeorge@icloud.com 	
Dafne Martínez: dafne@tipastype.com