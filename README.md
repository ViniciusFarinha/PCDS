
# Dashboard de Manutenção - Supervia

Antes de eu explicar o projeto, quero que vejam a imagem abaixo do painel principal do dashboard, para vocês terem uma ideia de como ficou. </br>


![Painel_Principal_PowerBI](https://user-images.githubusercontent.com/121468880/209687549-cf1b0296-71f2-4317-8593-906da1c0dad8.png)

##### Agora que já viram o resultado do projeto, vou explicar como ele foi feito. 

## O Projeto

Pra começar, de onde veio essa ideia? porque fazer um dashboard de controle de manutenção? </br>

Bom, a verdade é que a Supervia acabava de contratar uma empresa que ia realizar manutenção preditiva com um sistema vibracional.
Ou seja, estavamos prestes a ter um sistema que iria gerar diversos feedbacks pra empresa, em forma de dados, e precisávamos de uma forma de organizá-los e interpretá-los</br>

Esse sistema recebia o nome de **PCDS**.</br>

<p allign = 'center'>
<img  height = "300" src="Imagens\ImagemPCDS.jpeg">
</p>

Com a imagem acima podemos ver o sistema ligado ao pantógrafo do trem.</br>

## Primeiros Passos

A partir desse momento, meu gestor me deu a responsabilidade de cuidar dos dados gerados pelo sistema e de analisá-los. Esta foi a hora que eu fui em busca da base de dados gerada pelo sistema para entender como eu poderia atuar.</br>
<p allign = 'center'>
<img  width = "900" height = "240" src="Imagens\Telematica.png">
</p>


> Pois bem, está aí os dados na nuvem.

Logo, eu tive que pensar em uma forma de tabular esses dados de forma automatica para que eu otimizasse meu tempo. Assim, eu pensei em solucionar o problema da seguinte forma:
* Usar Selenium para captura de dados da Web;
* Utilizar o Pandas para tratamento de dados e tabulação em uma planilha do Excel;
* Realização de Dashboard e análises com os dados obtidos;
* Apresentação de resultados para gestores com e-mail automático.

</br>