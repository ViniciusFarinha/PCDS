
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


![Telematica](Imagens\Telematica.png)

> Pois bem, está aí os dados na nuvem.

Logo, eu tive que pensar em uma forma de tabular esses dados de forma automatica para que eu otimizasse meu tempo. Assim, eu pensei em solucionar o problema da seguinte forma:
* Usar Selenium para captura de dados da Web;
* Utilizar o Pandas para tratamento de dados e tabulação em uma planilha do Excel;
* Realização de Dashboard e análises com os dados obtidos;
* Apresentação de resultados para gestores com e-mail automático.
</br>

## Scrum

Depois de entender qual seria o plano, defini metas de entrega para o que eu estava lidando. Defini desta forma:
* Captura de dados da Web > 2 Semanas; 
* tratamento de dados e tabulação > 1 Semana;
* Dashboard  > 1 Semana;
* Resultados > 1 Semana.
</br>

## Selenium e a extração de dados

Utilizando a biblioteca do selenium, consegui fazer o login no site do sistema, clicar em alguns botões dentro da web e fazer o download do arquivo em CSV com os dados.

## Pathlib

O arquivo baixado estava indo diretamente para a pasta de download com um nome complexo e cheio de números de código. Com o pathlib, eu enviei o arquivo para a pasta do projeto com um nome mais fácil de identificar para codar: "Alarmes.xslx".</br>

## Pandas

Com a biblioteca do pandas eu tratei os dados do arquivo CSV para melhor visualização e análise.

## Dashboard - Power BI

Dado que o arquivo já estava tratado, esta era a hora de compilar os dados dentro de um dashboard.

## Win32com.client

Por fim, foi automatizado o envio da planilha de dados, junto com uma análise relatada manualmente no word.


## Conclusão

Depois de concluído, foi possível avaliar a situação da Rede Aérea dos trens da Supervia, otimizando a manutenção preditiva.Todos os arquivos do projeto estão dispostos no anexo.