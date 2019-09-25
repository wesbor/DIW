# Seccion 01: Ejemplo 01. Ejemplo border box

Ejemplo en el que se ven los cambios producidos por el cambio de tamaño en una caja al añadirle paddings y borders sin establecer la propiedad box-sizing: border box

Inicialmente la caja tendrá un tamaño de 20rem:

```
div{
    width: 20rem;
    height: 20rem;
    background-color:salmon;
}
```

Si añadimos un padding de 5rem, la caja pasará a medir 20+5*2=30rem

```
div{
    width: 20rem;
    height: 20rem;
    padding: 5rem;
    background-color:salmon;
}
```

Si añadimos un borde de 20px, tendremos 30rem+20px

```
div{
    width: 20rem;
    height: 20rem;
    padding: 5rem;
    background-color:salmon;
    border: 20px solid blue;
}
```

Si queremos fijar el tamaño de todo (caja original, padding y borde), hacemos
```
box-sizing: border-box;
```
https://www.w3schools.com/css/css3_box-sizing.asp
https://www.w3schools.com/cssref/css3_pr_box-sizing.asp

```
div{
    box-sizing: border-box; 
    width: 20rem;
    height: 20rem;
    padding: 5rem;
    background-color:salmon;
    border: 20px solid blue;
}
```

Si el texto se sale de la caja, tenemos 2 opciones
*overflow:hidden, que oculta todo el texto que no entre en la caja
*overflow: auto, que muestra una barra de scroll

```
div{
    box-sizing: border-box; 
    width: 20rem;
    height: 20rem;
    padding: 5rem;
    background-color:salmon;
    border: 20px solid blue;
    overflow: auto;
}
```