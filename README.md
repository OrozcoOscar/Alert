# Alert
Alerts/Modals


### _**alert**_
> Crea una alerta personalizada.
>
> **text:Obj** Recibe un objeto { title:String|HTML, contenido:String|HTML }.
> **opction:Obj** Configuracion de botones Ejem. [
> { name: "Aceptar", -> Nombre del Boton
> onclick:()=>{}, -> Accion a Realizar despues del Click
> type: 1 -> tipo de Boton [1,2,3,4,5]
> }]
>
> 
```javascript
Alert.alert({
        title:"Mi mensaje",
        contenido: `Hola Mundo`}, 
        [{
        name: "Cancelar",
        type: 3,
        onclick: () => { }
    },{
        name: "Peinar",
        type: 5,
        onclick: () => {}
    }, {
        name: "Aceptar",
        type: 1,
        onclick: () => {}
    }])
```
```javascript
let val
Alert.alert({
        contenido: `<h1>Ingrese El texto</h1>
        <input type="number" id="prompAlert">`}, 
        [{
        name: "Cancelar",
        type: 3,
        onclick: () => { }
    },{
        name: "Peinar",
        type: 5,
        onclick: () => {
    
         }
    }, {
        name: "Aceptar",
        type: 1,
        onclick: () => {
            val=document.querySelector("#prompAlert").value
          
        }
    }])
```
### _**prompt**_
> Crea una prompt.
>
> **text:Obj** Recibe un objeto { title:String|HTML, placeholder:String }.
> **opction:Obj** Configuracion de botones Ejem. [
> { name: "Aceptar", -> Nombre del Boton
> onclick:()=>{}, -> Accion a Realizar despues del Click
> type: 1 -> tipo de Boton [1,2,3,4,5]
> }]
>
> 
```javascript
let val
Alert.prompt({
    title: `Ingrese El texto`,
    placeholder:"ingresa algo aqui"
    },
    [{
        name: "Cancelar",
        type: 3,
        onclick: () => { }
    },{
        name: "Aceptar",
        type: 1,
        onclick: () => {
            val = document.querySelector("#PROMPTALERT").value
        }
    }])
```
