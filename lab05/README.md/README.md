
 LABORATORIO 05
-----------------


 TAREFA 01
--------------
No link do Google Drive modelo ou no diretório resources/ você encontrará um modelo para resolver a tarefa:

Escolha um conjunto de componentes do laboratório passado e os represente na forma de componentes com sub-comopnentes.


Tarefa 02
---------------
Crie uma conta no Codepen, copie o código do exemplo React 03 - Componente Barra para a sua conta e construa um exemplo de componente adaptando o exemplo apresentado. Por se tratar de programação em JavaScript, podem ser feitas adaptações bastante simples.

* HTML
~~~html
<div id="root"></div>
~~~


* JavaScript
~~~jss
class Barra extends React.Component {
  render() {
    let resultado = "";
    for (let b = 1; b <= this.props.tamanho; b++)
      resultado += "=";
    return resultado;
  }
}

const elemento = <div>
                   <h2>O dinossauro</h2>
                   <Barra tamanho="10"/>
                   <h2>pulou na lama.</h2>
                 </div>
ReactDOM.render(elemento, 
        document.getElementById("root"));

ReactDOM.render(
 <h1>Tricerátops Pertencia a espécie triceratopis horridus. Altura = 2 metros e largura 9 metros.</h1>,
 document.getElementById("root")
);

~~~
