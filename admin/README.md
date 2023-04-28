# Anotações do Projeto
Depois de baixar a pasta:
- npm install

## Para criar um cliente 
Criei uma função que receberá dois paramêtros nome e e-mail:

````js
    const criaNovaLinha = (nome, email) => {
    const linhaNovoCliente = document.createElement('tr')
    const conteudo = `
        <td class="td" data-td>${nome}</td>
        <td>${email}</td>
        <td>
            <ul class="tabela__botoes-controle">
                <li><a href="../telas/edita_cliente.html" class="botao-simples botao-simples--editar">Editar</a></li>
                <li><button class="botao-simples botao-simples--excluir" type="button">Excluir</button></li>
             </ul>
        </td>`
    linhaNovoCliente.innerHTML = conteudo;
    return linhaNovoCliente;
}
````

abrir a pasta admin no vscode e 
rodar o json server: 
```js
json-server --watch db.json
```

Rodar: browser-sync start --server --file . --host --port 5000 --startPath admin/telas/lista_cliente.html
