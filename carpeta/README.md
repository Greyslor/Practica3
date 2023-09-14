# Practica 3: Git

## Datos Personales

- **Nombre**: Grecia Lorena Morales Castillo
- **Edad**: 20 años

![Greys](/carpeta/img/greys.jpg)

Enlace al cuestionario de la Práctica 5 ![practica5](/carpeta/practica-5.md)


**Principios de Composición y Diseño**
- **Profesor**: Roberto Melo
- Conocer los principios, técnicas y campos de aplicación del diseño gráfico y la composición, y ser capaz de aplicarlas mediante las herramientas adecuadas en soporte digital para resolver problemas visuales y diseñar interfaces gráficas efectivas que transmitan, con suficiente calidad técnica, un mensaje o una idea a través de contenido visual adecuadamente estructurado según la sintaxis y morfología propia del lenguaje del diseño gráfico.

**Diseño de Videojuegos**
- **Profesor**: Hector Guerrero
- Conocer las técnicas, los elementos y los artefactos empleados en la concepción de un videojuego, y ser capaz de utilizarlos para concebir nuevos juegos, razonando sobre las fortalezas y debilidades de éstos, y generando documentos formales de diseño de juegos en los que dichos artefactos sean correctamente estructurados y comunicados.
 DiseñoVideojuegos

**Sistemas Operativos y Redes**
- **Profesor**: Osiel Morales
- Estructura de los sistemas operativos (software). Aplicación de redes.

**Lenguajes Interpretados**
- **Profesor**: Jonathan Miranda
- Conocer y saber aplicar la programación con los lenguajes interpretados más utilizados en el ámbito de la programación de aplicaciones interactivas, para adentrarse en la metodología de programación lógica de mecánicas de juego de alto nivel, control de interfaces gráficas y scripting de unidades funcionales independientes dentro de programas de complejidad elevada.


**Proyecto Semestral: Desarrollo de Aplicaciones Interactivas**
- Profesor: Sebastian Mejia
- Conocer los conceptos elementales de la programación por computadora en los lenguajes C y C++, tanto en el ámbito del diseño algorítmico como en el de estructuración y desarrollo de software, implementar programas de tamaño medio, evaluando su corrección y eficiencia y ser capaz de identificar y abstraer los contenidos importantes de los problemas reales para elegir las soluciones mas eficientes para poder afrontar el diseño de programas de complejidad media, independientemente del lenguaje de programación a utilizar.


**Inglés Técnico Para Videojuegos III**
- **Profesora**: Angie
- Aprendizaje de inglés, mejorar vocabulario, gramática, lenguaje.

# Parcial 2 

## Práctica 1
Agregando un cambio 12 septiembre 2023
shfishyeifhsoe
sijhdfkloij


## Práctica 2

**¿Cómo se inicializa un repositorio en Git?**

Para inicializar en un repositorio local se ocupan los siguientes comandos en la terminal del programa usado: 

```js
mkdir carpeta
cd carpeta
touch README.md
touch .gitignore
git init
code .
```
De igual manera usar la rama main configurando lo siguiente:

```js
git init
git add .
git commit -m "Primer commit"
git branch -M main
git remote add origin https://github.com/usuario/repositorio.git
git push -u origin main
```

**¿Cómo creas un repositorio en GitHub?**

Primero que nada es necesario tener una cuenta en la página de GitHub. Al ingresar a la interfaz, podemos ver que hay un ícono de "nuevo" con el símbolo de un libro, dar click ahí y nos cargará la nueva pantalla para crearlo. Le ponemos un nombre, una descripción (opcional), seleccionamos si será público o privado, podemos agregar de una vez un readme, un gitignore o una licencia, o agregarlas después. Y por último dar click en crear repositorio.


**¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?**

Desde otro computador es necesario configurar git antes usando los siguientes comandos:

```js
git --version
git config --global user.name "Name"
git config --global user.email example@gmail.com
git config --global user.ui true
git config --global init.defaultBranch main
git config --list
# asignando visual studio code como editor de configuración de git
git config --global core.editor "code --wait"
git config --global -e
```

Después clonas el repositorio creado usando el comando
```js
git clone https://github.com/usuario/repositorio.git
```
Puedes seguir subiendo cambios desde la rama main o crear otra.

**¿Cuál es el flujo básico de trabajo en Git y GitHub?**

**_Moodified_**  Es la carpeta local de la computadora donde se almacenan los archivos del proyecto.
Es como un guardar sencillo, "ctrl + s".

**_Stage_** Es el área donde git indexa y agrega los cambios realizados en los archivos previos, antes de comprometerlos en el registro. Se usa:

```js
git add .
```

**_Local Repository_**: Los cambios ya se registran en el repositorio de git. Subiendo los cambios usando:

```js
git commit -m "example commit"
```

**_Remote Repository_**: Es el área donde trabaja el directorio remoto donde almacenamos los archivos del proyecto.

```js
git push
```
**_Git Pull_** Igualmente para jalar algún archivo o cambio se usa:

```js
git pull 
```