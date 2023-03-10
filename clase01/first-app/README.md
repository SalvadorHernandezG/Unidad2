# Creando la primera aplicación con Angular 51
En ésta primera clase se trabajará con el carrito de compra pero practicando con la Introducción a Angular.

![image](https://user-images.githubusercontent.com/8560750/210269435-d113f722-31ad-4e1b-8a5c-e30da120059b.png)


## Ejecutar el comando para crear la aplicación
~~~
ng new first-app
~~~

## Responder a las preguntas
![image](https://user-images.githubusercontent.com/8560750/210268348-f274a186-4e06-434f-8095-21f17f92cd25.png)

## Configurar el proyecto con PrimeNG
Véase referencia de [PrimeNG](https://primeng.org/setup)

### Instalar las dependencias en el proyecto
~~~
npm install primeng --save
npm install primeicons --save
~~~

### Configurar el archivo angular.json en la sección Styles

~~~
            "styles": [
              "src/styles.css",
              "node_modules/primeicons/primeicons.css",
              "node_modules/primeng/resources/themes/md-light-indigo/theme.css",
              "node_modules/primeng/resources/primeng.min.css"              
            ],

~~~



## Ejecutar la aplicación
### Cambiarse al directorio de trabajo
~~~
cd first-app
~~~

### Ejecutar el comando para levantar el servidor
~~~
ng serve
~~~

### Abrir el navegador web e ingresar la URL
~~~
http://localhost:4200/
~~~

## Creando un nuevo componente
### Cambiar la configuración de angular.json
![image](https://user-images.githubusercontent.com/8560750/210268549-8cf883ad-7696-42d9-a913-21dea5e695d8.png)

### Ejecutar los comandos para crear el componente Header y Footer
~~~
ng g c header
ng g c footer
~~~
![image](https://user-images.githubusercontent.com/8560750/210268601-e158f8f6-1493-428b-baec-03c2be47e14e.png)


## Modificar el componente HEADER
### Modificar el archivo app.component.html
~~~
<app-header></app-header>
<div class="content">
    <h1>Introducción a Angular</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, veniam ducimus laborum dignissimos perferendis ut, molestias placeat dicta recusandae nam fugiat magni cumque nobis nisi perspiciatis qui reprehenderit deserunt quibusdam.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, veniam ducimus laborum dignissimos perferendis ut, molestias placeat dicta recusandae nam fugiat magni cumque nobis nisi perspiciatis qui reprehenderit deserunt quibusdam.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, veniam ducimus laborum dignissimos perferendis ut, molestias placeat dicta recusandae nam fugiat magni cumque nobis nisi perspiciatis qui reprehenderit deserunt quibusdam.</p>
</div>
<app-footer></app-footer>
~~~

### Modificar el archivo app.component.css
~~~
.content {
    background-color: aliceblue;
    min-height: calc(100vh - 60px);
}
~~~

### Modificar el archivo header.component.css
```
:host {
    background-color: rgb(18, 135, 238);
    color: white;
    border-radius: 5px;
    display: block;
    font-size: 2rem;
    height: 40px;
    margin-bottom: 5px;
    text-align: center;
    padding: 5px;
}
```

### Modificar el archivo footer.component.css
```
:host {
    background-color: rgb(18, 135, 238);
    border-radius: 5px;
    color: white;
    display: block;
    font-size: 0.8rem;
    height: 20px;
    text-align: center;
}
```

### Modificar el archivo styles.css
```
* {
    margin: 0px;
    padding: 0px;
}
```

## Conceptos de la práctica con tus propias palabras
- Define que es un `componente` y al crearlo que elementos lo forman.
- Define que es un `módulo` y que función tiene el patrón de diseño decorator.
- Menciona y describe los elementos importantes de un @NgModule
- Subir tu práctica al [GitHub](https://github.com/) y comparte en la entrega de [Elearning](https://elearning.utng.edu.mx/) en la entrega correspondiente de la Unidad 2.
- Modificar el componente que tenga el atributo titulo y en el constructor asignarle el valor "Welcome tu Angular"; en el componente HTML invocar el atributo titulo.
- Crear un Layout donde se despliegue el Header con una barra de menús, no se te olvide el estilo.
- Igualmente invocar el componente Footer dentro del layout, no se te olvide el estilo.
- Define una clase que se llame **Usuario** con los atributos email, contraseña y métodos login y register.
- Desplegar la aplicación en [StackBlitz](https://stackblitz.com/).
