<template>
<div id="form">
  <div class="container">
    <h1>Tela de cadastro de clientes</h1>

    <form>
    <h3>DADOS PESSOAIS</h3>
      <label for="cpf">Insira seu CPF: </label>
      <input type="text" id="cpf"><br><br>

      <label for="nome">Nome: </label>
      <input type="text" id="nome"><br><br>

      <label for="rg">RG: </label>
      <input type="text" id="rg"><br><br>

      <label for="data-expedicao">Data de expedicao: </label>
      <input type="date" id="data-expedicao"><br><br>

      <label for="orgao-expedicao">Orgão de expedicao: </label>
      <input type="text" id="orgao-expedicao"><br><br>

      <label for="uf-expedicao">UF: </label>
      <input type="text" id="uf"><br><br>

      <label for="data-nascimento">Data de nascimento: </label>
      <input type="date" id="data-nascimento"><br><br>

      <label for="sexo">Sexo: </label>
      <input type="text" id="sexo"><br><br>

      <label for="estado-civil">Estado civil: </label>
      <input type="text" id="estado-civil"><br><br>

      <h3>ENDEREÇO</h3>
      <label for="cep">CEP: </label>
      <input type="text" id="cep"><br><br>

      <label for="logradouro">Logradouro: </label>
      <input type="text" id="logradouro"><br><br>

      <label for="numero">Número: </label>
      <input type="text" id="numero"><br><br>

      <label for="complemento">Complemento: </label>
      <input type="text" id="complemento"><br><br>

      <label for="bairro">Bairro: </label>
      <input type="text" id="bairro"><br><br>

      <label for="cidade">Cidade: </label>
      <input type="text" id="cidade"><br><br>

      <label for="uf-endereco">UF: </label>
      <input type="text" id="uf-endereco"><br><br>
      <button>Salvar</button>
    </form>

    <table>
      <thead>
        <tr>
          <th>CPF</th><br><br>
          <th>Nome</th>
          <th>RG</th>
          <th>Data de expedição</th>
          <th>Orgão de expedição</th>
          <th>UF</th>
          <th>Data de nascimento</th>
          <th>Sexo</th>
          <th>Estado civil</th>
          <th>CEP</th>
          <th>Logradouro</th>
          <th>Número</th>
          <th>Complemento</th>
          <th>Bairro</th>
          <th>Cidade</th>
          <th>UF</th>
          <th>Opções</th>
        </tr>
      </thead>

      <tbody>
        <tr>
          <td>11</td>
          <td>Lucas</td>
          <td>395902</td>
          <td>02/20/2002</td>
          <td>SSP</td>
          <td>SP</td>
          <td>02/12/2300</td>
          <td>M</td>
          <td>Solteiro</td>
          <td>04854</td>
          <td>Rua</td>
          <td>187</td>
          <td>Casa</td>
          <td>Jd</td>
          <td>São paulo</td>
          <td>SP</td>
          <td>
          <a href="/"><button><img alt="alterar" id="alterar" src="../images/change.png"></button></a>
          <a href="/"><button><img alt="deletar" id="deletar" src="../images/delete.png"></button></a>
          </td>


        </tr>
      </tbody>

    </table>

  </div>
</div>
</template>


<style scoped>
   <style scoped>
    #form{
        display: flex;
        align-items: center;
  

    }

    .container{
        display: flex; 
        align-items: center;
        flex-direction: column;
    }
</style>


