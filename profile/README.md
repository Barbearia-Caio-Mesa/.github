<h3 align="center">
  <img src="../assets/logo_caio_mesa.jpg" alt="logo-Sistema" >
</h3>

# Sistema de Agendamentos - Caio Mesa Barbearia
<p align="center">
  Um sistema completo de <b>gestão e agendamento para a barbearia do Caio Mesa</b>, com foco em <b>automação de atendimento</b>, <b>controle financeiro</b> e <b>melhoria da experiência do cliente</b>.
</p>

<p align="center">
     <a href="#">
        <img 
           alt="Localização" 
            title="Localização São Paulo - BR" 
            src="https://custom-icon-badges.demolab.com/badge/S%C3%A3o%20Paulo-BR-green?style=for-the-badge&logo=location&logoColor=white"
        />
    </a>
</p>
<p align="center">
    <a href="https://github.com/Barbearia-Caio-Mesa/Sistema-Interface-Frontend">
        <img 
            alt="frontend" 
            title="Repositório - Frontend" 
            src="https://custom-icon-badges.demolab.com/badge/Interface-Frontend-blue?style=for-the-badge&logo=react&logoColor=white"
        />
    </a> 
    <a href="https://github.com/Barbearia-Caio-Mesa/Sistema-API-Core">
        <img 
            alt="api-core" 
            title="Repositório - API Core" 
            src="https://custom-icon-badges.demolab.com/badge/API-Core-green?style=for-the-badge&logo=nodedotjs&logoColor=white"
        />
    </a>
</p>

<p align="center">
    <a href="https://github.com/Barbearia-Caio-Mesa/Servico-Autenticacao-Segura">
        <img 
            alt="auth-jwt" 
            title="Repositório - Autenticação" 
            src="https://custom-icon-badges.demolab.com/badge/Autenticação-JWT-black?style=for-the-badge&logo=jsonwebtokens&logoColor=white"
        />
    </a> 
    <a href="https://github.com/Barbearia-Caio-Mesa/Infraestrutura-Banco-Dados">
        <img 
            alt="database" 
            title="Repositório - Banco de Dados" 
            src="https://custom-icon-badges.demolab.com/badge/Banco-Dados-Dados?style=for-the-badge&logo=jsonwebtokens&logoColor=white"
        />
    </a>
</p>

## 🚨 Problema
- Agendamentos realizados principalmente via WhatsApp, o que causa dificuldade para visualizar a agenda do dia e falta de organização dos serviços.
- Ausência de um controle claro sobre a utilização de pacotes de serviços (ex: pacote mensal de 4 cortes ou combos de cabelo e barba), gerando confusão.
- Clientes que esquecem do horário marcado, resultando em horários vagos e perda financeira para o profissional.
- Dificuldade do barbeiro em acompanhar o controle financeiro de entradas e saídas de dinheiro do negócio.

## 💡 Solução
- Sistema de agendamento online direto pelo site, com menu de serviços e valores bem definidos, evitando conflitos de horários.
- Integração com o WhatsApp para o envio de lembretes automáticos aproximadamente 1 hora antes do agendamento, reduzindo faltas.
- Dashboard financeira semanal para o barbeiro acompanhar o total arrecadado, a quantidade de atendimentos e os serviços mais solicitados.
- Portfólio visual e galeria de fotos de cortes já realizados para atrair novos clientes, além de um perfil detalhado do barbeiro com avaliações.
- Implementação de pagamento digital via Pix e um sistema de "Corte Presente" (vouchers) para presentear outras pessoas.

## 🗂️ Estrutura da Organização
Este projeto foi arquitetado com foco em escalabilidade na nuvem e está dividido nos seguintes repositórios:  

- 📂 [Sistema-Interface-Frontend](../Sistema-Interface-Frontend) → Aplicação web responsiva (Hospedada via AWS S3 / CloudFront).  
- 📂 [Sistema-API-Core](../Sistema-API-Core) → API RESTful principal para gestão de regras de negócio (AWS EC2).  
- 📂 [Servico-Autenticacao-Segura](../Servico-Autenticacao-Segura) → Módulo de segurança e identidade utilizando JWT.
- 📂 [Infraestrutura-Banco-Dados](../Infraestrutura-Banco-Dados) → Modelagem e scripts do banco de dados relacional.
- 📂 [.github](../.github) → Documentação geral da organização e configurações.  

## ⚙️ Tecnologias
<div style="display: flex; gap: 10px; flex-wrap: wrap;">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" title="JavaScript" width="50px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" title="Node.js" width="50px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" title="Node.js" width="50px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" title="MySql" width="50px"/>
  <img src="../assets/aws.svg" title="AWS" width="50px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" title="Git" width="50px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" title="GitHub" width="50px"/>
</div>

## 🌐 Arquitetura do Sistema
- 📱 **Interface Web (Frontend)** → SPA focada em UX, consumindo a API para exibição de horários, galeria de cortes e agendamentos.
- ⚙️ **Backend (API Core)** → Processamento de regras de negócios, controle de pacotes e gestão financeira. Hospedado em instância **AWS EC2**.
- 🔐 **Autenticação (JWT)** → Microsserviço responsável por garantir a segurança das rotas administrativas do barbeiro e acesso de clientes.
- 🗄️ **Banco de Dados** → Armazenamento relacional e seguro de usuários, agendamentos e histórico financeiro.
- 💬 **Integrações** → Comunicação com API do WhatsApp para automação de lembretes e API do Pix para pagamentos.

## ✒️ Equipe

<table>
  <tr>
    <td align="center" width="160px">
      <a href="https://github.com/CatarinaGimenes">
        <img src="https://avatars.githubusercontent.com/u/199615487?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Catarina Gimenes Pires</b>
      </a><br /> 
      <sub> Arquiteta de Soluções</sub> <br/>
    </td>
    <td align="center" width="160px">
      <a href="https://github.com/JhoelDiego2">
        <img src="https://avatars.githubusercontent.com/u/198672530?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Jhoel Diego M. Mita</b>
      </a><br /> 
      <sub> Arquiteto Técnico </sub> <br/>
    </td>
    <td align="center" width="160px">
      <a href="https://github.com/ThaisKheyla">
        <img src="https://avatars.githubusercontent.com/u/198767592?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Kheyla Thais Q. Paucara</b>
      </a><br /> 
      <sub> Engenheira de Software </sub> <br/>
    </td>
  </tr>
  <tr>
    <td align="center" width="160px">
      <a href="https://github.com/LukasFah">
        <img src="https://avatars.githubusercontent.com/u/199182791?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Lukas F. de Oliveira</b>
      </a><br /> 
      <sub> Desenvolvedor Back-End </sub> <br/>
    </td>
    <td align="center" width="160px">
      <a href="https://github.com/Rfratini">
        <img src="https://avatars.githubusercontent.com/u/199615576?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Rafael F. Dal Corso</b>
      </a><br /> 
      <sub> Engenheiro de Software </sub> <br/>
    </td>
    <td align="center" width="160px">
      <a href="https://github.com/RenanDaher1">
        <img src="https://avatars.githubusercontent.com/u/199526561?v=4" style="border-radius:50%;" width="100px;"/><br/>
        <b>Renan D. Franceschelli</b>
      </a><br /> 
      <sub> Engenheiro de Dados </sub> <br/>
    </td>
  </tr>
</table>