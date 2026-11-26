<script>
  export let numero;   // se exporta para usarla desde App.svelte
  let resultado;       // variable local
  $: if (numero === 0)           // $: da reactividad
       resultado = "neutro";
     else if (numero % 2 === 0)
       resultado = "par";
     else
       resultado = "impar";
</script>

<p>El número {numero} es {resultado}</p>

<style>
  p {
    color: rgb(34, 5, 112);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 25px;
  }
</style>