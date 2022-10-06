<p align="center"> <img src="./logo/logofinal.png" alt="CATE" class="center" width=300/> </p>

<h1 align="center">CATE - Coleta Análise Tratamento Exibição</h1>

O projeto a ser desenvolvido vai ser um sistema de gestão de reconciliação de planos de saúde para a empresa parceira [Dom Rock](https://www.domrock.net/) juntamente com a Faculdade de Tecnologia de São José dos Campos Professor Jessen Vidal.

<h2 align="center">📋 Tabela de conteúdos</h2>

<!--ts-->
   * [Introdução](#cate---coleta-análise-tratamento-exibição)
   * [Features](#-features)
   * [Demonstração da aplicação](#-demonstração-da-aplicação)
   * [Projeto](#-projeto)
   * [Desafio](#-desafio)
   * [Solução](#-solução)
   * [Entregas](#-entregas)
   * [Rodando o Sistema](#-rodando-o-sistema)
   * [Tecnologias](#-tecnologias)
   * [Membros](#-membros)
   * [Licença](#-licença)
   * [Dicionário do projeto](#-Dicionário-do-Projeto)
<!--te-->

<h2 align="center">✅ Features</h2>

- [x] Níveis de processamento dos dados Bronze e Silver
- [x] Extração dos dados
- [x] LOG do processo de extração dos dados
- [ ] Limpeza dos dados
- [x] Armazenamanto dos dados brutos no MongoDB
- [x] Log do processo de persistência no MongoDB
- [ ] Cruzamento dos dados
- [ ] Armazenamento dos dados cruzados no MongoDB
- [ ] Armazenamento dos dados cruzados no DW
- [ ] Aplicação da LGPD
- [ ] Relatórios no Power BI
- [ ] Bônus
  - [ ] Implementação Machine Learning

<h2 align="center">📺 Demonstração da aplicação</h2>

<p align="center">Demonstração dos protótipos de relatório</p>

<div align="center">

![Alt Text](./demonstracao-aplicacao/grafico-1.png)
![Alt Text](./demonstracao-aplicacao/grafico-2.png)
![Alt Text](./demonstracao-aplicacao/grafico-3.png)

</div>

<h2 align="center">🖥 Projeto</h2>

Projeto realizado em parceria com a Dom Rock que disponibiliza uma plataforma permite a captura de dados não estruturados e estruturados de forma automatizada e promove a visualização otimizada de análises, informações e dados que viabilizam ganhos recorrentes para diversas áreas de negócios das empresas. A plataforma foi projetada e construída com tecnologias mais avançadas de big data e inteligência artificial com arquitetura de nuvem auto escalável. Nos últimos anos a plataforma tem sido reconhecida como uma das melhores do Brasil por rankings qualificados e através de programas de inovação aberta de grandes corporações e organizações.

<h2 align="center">📈 Desafio</h2>

Desafio proposto pela Dom Rock - O cliente gerencia um sistema de gestão de planos de saude que possui a seguinte necessidade: Uma solução que concilie as informações oriundas de demonstrativo de uma operadora de saúde e a lista de beneficiários dos planos de saúde dessa operadora para cada competência (mensal). Como os dados contém dados pessoais é mandatório a aplicação de regras LGPD para efeito de auditoria.

<h2 align="center">💡 Solução</h2>

CATE é o projeto que possibilita um melhor gerenciamento dos dados, permitindo melhor desempenho, integridade, segurança e privacidade dos mesmos.
Com um bom fluxo dos dados definido é possivel gerar relatórios de discrepâncias e exibi-las ao controlador permitindo a rapida correção.

<h2 align="center">💎 Entregas</h2>

Abaixo segue o planejamento e o progresso durante as Sprints do projeto.

|   **SPRINT**    |  **DATA DE ENTREGA**  | **O QUE SERÁ ENTREGUE** |
|-----------------|-----------------------|-------------------------|
|  1  |  29/08/2022 a 18/09/2022  | Modelagem dos dados, níveis de processamento dos dados (Bronze e Silver), extração dos dados das bases, LOG do processo de extração, persitência dos dados brutos no MongoDB, LOG do processo de persistência no MongoDB.
|  2  |  19/09/2022 a 09/10/2022  | Limpeza dos dados extraídos das bases, analíse e cruzamento dos dados via Python e persitência dos dados cruzados no MongoDB.
|  3  |  13/10/2022 a 06/11/2022  | Aplicação da LGPD, modelagem e implementação do DW, Persitência dos dados relevantes no DW.
|  4  |  07/11/2022 a 27/11/2022  | Modelagem e implemantação do Power BI, integração entre o DW e o Power BI, relatórios no Power BI e Machine Learning (bônus).

<h2 align="center">🚀 Rodando o Sistema</h2>

<h3>📑 Pré-requisitos</h3>

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com), [Python](https://www.python.org/)  e [PIP](https://pypi.org/project/pip/).
Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/) ou [PyCharm](https://www.jetbrains.com/pt-br/pycharm/).

<h3>🎲 Rodando o Python</h3>

```bash
# Clone este repositório
$ git clone https://github.com/API-6-SEMESTRE/Projeto

# Rodar o comando a seguir no terminal para instalar as bibliotecas do PIP
$ pip install -r src/requirements.txt

# Rodar um dos comandos a seguir:

## Nível BRONZE - Extração dos dados das planilhas e a persistência no MongoDB SEM anonimizar os dados
$ python3 src/et_l.py -l bronze

## Nível SILVER - Extração dos dados das planilhas e a persistência no MongoDB COM anonimização dos dados
$ python3 src/et_l.py -l silver

# Pronto! Os dados foram persistidos no MongoDB de acordo com a opção escolhida.
```


<h2 align="center">🛠 Tecnologias</h2>

As seguintes ferramentas foram usadas na construção do projeto:

<p align="center">
 <a href="https://www.mongodb.com/">
  <img src="https://img.shields.io/static/v1?label=MongoDB&message=Banco de Dados NoSQL&color=47A248&style=for-the-badge&logo=mongodb"/>
 </a>
 <a href="https://www.mysql.com/">
  <img src="https://img.shields.io/static/v1?label=MySQL&message=Banco de Dados Relacional&color=4479A1&style=for-the-badge&logo=mysql"/>
 </a>
 <a href="https://powerbi.microsoft.com/pt-br/">
  <img src="https://img.shields.io/static/v1?label=Power BI&message=Relatórios&color=F2C811&style=for-the-badge&logo=Power BI"/>
 </a>
</p>
<p align="center">
  <a href="https://www.python.org/">
  <img src="https://img.shields.io/static/v1?label=Python&message=Análise de Dados&color=3776AB&style=for-the-badge&logo=Python"/>
</a>
<a href="https://pandas.pydata.org/">
  <img src="https://img.shields.io/static/v1?label=Pandas&message=Análise de Dados&color=150458&style=for-the-badge&logo=pandas"/>
</a>
<a href="https://pypi.org/project/pip/">
  <img src="https://img.shields.io/static/v1?label=PIP&message=Análise de Dados&color=3775A9&style=for-the-badge&logo=PyPI"/>
</a>
</p>
<p align="center">
  <a href="https://git-scm.com/">
  <img src="https://img.shields.io/static/v1?label=Git&message=DevOps&color=F05032&style=for-the-badge&logo=Git"/>
</a>
  <a href="https://github.com/">
  <img src="https://img.shields.io/static/v1?label=GitHub&message=DevOps&color=181717&style=for-the-badge&logo=GitHub"/>
</a>
<a href="https://www.atlassian.com/br/software/jira">
  <img src="https://img.shields.io/static/v1?label=Jira&message=Processo&color=0052CC&style=for-the-badge&logo=Jira Software"/>
 </a>
 <a href="https://www.microsoft.com/pt-br/microsoft-teams/log-in">
  <img src="https://img.shields.io/static/v1?label=Microsoft Teams&message=Processo&color=6264A7&style=for-the-badge&logo=Microsoft Teams"/>
 </a>
</p>

<h2 align="center">👥 Membros</h2>

<table align="center">
    <tr>
        <td align="center">
            <a href="https://linkedin.com/in/tairik-nishimura/">
                <img style="border-radius: 50%;" src="./fotos/tairik.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Tairik Johnny</b>
                </sub>
            </a>
            <br />
            <p>Scrum Master</p>
            <a href="[https://www.mongodb.com/](https://linkedin.com/in/tairik-nishimura/)">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/maxx-barcelos-aaa106b2/">
                <img style="border-radius: 50%;" src="./fotos/maximiles.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Maximiles Barcelos</b>
                </sub>
            </a>
            <br />
            <p>Product Owner</p>
            <a href="https://www.linkedin.com/in/maxx-barcelos-aaa106b2/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/jeferson-tadeu-das-neves-a98343190/">
                <img style="border-radius: 50%;" src="./fotos/jeferson.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Jeferson Neves</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/jeferson-tadeu-das-neves-a98343190/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://linkedin.com/in/devanir-ramos-junior/">
                <img style="border-radius: 50%;" src="./fotos/devanir.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Devanir Ramos</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://linkedin.com/in/devanir-ramos-junior/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
    </tr>
    <tr>
        <td align="center">
            <a href="https://www.linkedin.com/in/jos%C3%A9-francisco-forneiro-junior/">
                <img style="border-radius: 50%;" src="./fotos/jose.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>José Francisco</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/jos%C3%A9-francisco-forneiro-junior/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/alan-bezerra/">
                <img style="border-radius: 50%;" src="./fotos/alan.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Alan Lucas</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/alan-bezerra/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/leonardo-gabriel-silva-11b8b8178/">
                <img style="border-radius: 50%;" src="./fotos/leonardo.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Leonardo Gabriel</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/leonardo-gabriel-silva-11b8b8178/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
        <td align="center">
            <a href="https://www.linkedin.com/in/henrique-zucareli-santiago/">
                <img style="border-radius: 50%;" src="./fotos/henrique.png" width="150px;" height="150px;" alt="image" />
                <br />
                <sub>
                    <b>Henrique Zucareli</b>
                </sub>
            </a>
            <br />
            <p>Developer</p>
            <a href="https://www.linkedin.com/in/henrique-zucareli-santiago/">
              <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
            </a>
        </td>
    </tr>
</table>

<h2 align="center">📝 Licença</h2>

Todas as informações resultantes da Aprendizagem por Projetos Integrados da Fatec São José dos Campos - Prof. Jessen Vidal seguem a licença Open Source Initiative (OSI) ou Academic Free License 3.0 (AFL-3.0).
