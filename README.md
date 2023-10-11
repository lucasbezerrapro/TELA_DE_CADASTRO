# TELA_DE_CADASTRO
let login = function() {
  // Obtenha os valores dos campos de entrada
  let nomeInput = document.getElementsByClassName("nome")[0].value;
  let senhaInput = document.getElementsByClassName("senha")[0].value;

  let banco_dados = {
    'senhas': ['12345', '33445566'],
    'nomes': ['lucas', 'pedro', 'jonas']
  };

  // Verifique se o nome e senha inseridos existem nos arrays
  if (banco_dados['nomes'].includes(nomeInput) && banco_dados['senhas'].includes(senhaInput)) {
    alert("Login bem-sucedido :)");
  } else {
    alert("Senha ou nome incorretos. Tente novamente.");
  }
}


let corOutline = () => {
  document.getElementsByClassName("nome").style.outlineColor = "red";
} 
