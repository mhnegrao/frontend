<script>
import FormAtividade from "./componentes/form-atividade.svelte";
import GridAtividade from "./componentes/grid-atividade.svelte";
import PopWindow from "./componentes/pop-window.svelte";

  export let name;
</script>
<div class="window">
<main>
  <div class="panel">
    <h1>Olá {name}, Bem Vindo !!!</h1>
    <h2>Controle de Atividades</h2>
    <!-- <p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p> -->
    <div id="barra-titulo">
      <h3>Você tem (x) atividades</h3>
    </div>
  </div>
  <div id="barra-menu">
    <button id="novo" class="btn btn-primary">Novo</button>
    <button id="novo" class="btn btn-primary">Editar</button>
    <button id="novo" class="btn btn-primary">Pesquisar</button>
    <button id="novo" class="btn btn-default">Exluir</button>
    <button id="novo" class="btn btn-danger">Sair</button>
  </div>
  <p></p>
  <GridAtividade/>
</main>

</div>
<FormAtividade/>
<PopWindow/>
<style>
  main {
    text-align: center;
	text-shadow: #ff3e00;
	font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }
  .panel {
    background-color: white;

  }
  .window{
	  border-radius: 3px;
	  border-style:double;
	  
  }
  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
