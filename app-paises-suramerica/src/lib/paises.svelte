<script>
    export let pais;
    let p;
    const paises={
        "colombia":["colombia","bogota","51,52 millones","peso colombiano","1,142 km","Flag_of_colombia.svg"],
        "venezuela":["venezuela","caracas","28,2 millones","bolivar","916,445 km","Flag_of_venezuela.svg"],
        "ecuador":["ecuador","quito","17,8 millones","dolar estaunidense","256.370 km","Flag_of_ecuador.svg"],
        "peru":["peru","lima","33,72 millones","sol peruano","1.285.215 km","Flag_of_peru.svg"],
        "brasil":["brasil","brasilia","214,3 millones","real brasileno","8,51 km","Flag_of_brazil.svg"]
    }
    p=paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img src="./src/assets/{p[5]}" alt="bandera_colombia" width="300" height="300">
    </div>
    <div class="col2">
        <div class="linea"><strong>pais</strong></div>
        <div class="linea"><strong>capital</strong></div>
        <div class="linea"><strong>poblacion</strong></div>
        <div class="linea"><strong>moneda</strong></div>
        <div class="linea"><strong>extension</strong></div>
    </div>
</div>
<style>
    .main{
        display: grid;
        grid-template-columns: repeat(4,1fr);
        grid-gap: 5px;
        grid-auto-rows: minmax(100px,auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(186, 190, 182);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
    }

    .col1{
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width: max-content;
    }
    strong{
        color: blue;
        font-weight: bolder;
    }
    .linea{
        font-size: 20px;
        margin-bottom: 18px;
    }
</style>