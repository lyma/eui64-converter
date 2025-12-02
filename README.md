<div align="center">

<img src="https://www.google.com/search?q=https://img.shields.io/badge/Network-Tools-blue%3Fstyle%3Dfor-the-badge%26logo%3Dcisco%26logoColor%3Dwhite" alt="Network Tools" />






⚡ Conversor EUI-64 (MAC ↔ IPv6)

Uma ferramenta moderna, elegante e responsiva para engenheiros de rede e desenvolvedores.

<p>
<a href="#-funcionalidades">Funcionalidades</a> •
<a href="#-tecnologias">Tecnologias</a> •
<a href="#-como-usar">Como Usar</a> •
<a href="#-lógica-eui-64">Lógica EUI-64</a>
</p>

<!-- SUBSTITUA O LINK ABAIXO PELA URL DO SEU PRINT QUANDO SUBIR A IMAGEM -->

<!-- <img src="./preview.png" alt="Preview da Aplicação" width="800"> -->

</div>

📖 Sobre o Projeto

Este projeto é uma aplicação web Single Page (SPA) leve e autônoma projetada para converter endereços físicos (MAC) em endereços IPv6 Link-Local usando o padrão EUI-64, e realizar o processo inverso.

O foco principal foi criar uma UI/UX premium, utilizando conceitos de Glassmorphism, gradientes modernos e feedbacks visuais intuitivos, fugindo das ferramentas de rede com visual antigo.

✨ Funcionalidades

🔄 Conversão Bidirecional:

MAC para IPv6: Gera o endereço Link-Local (fe80::) e o Interface ID.

IPv6 para MAC: Recupera o MAC Address original a partir de um IPv6 EUI-64.

🎨 UI Moderna (Glassmorphism): Design translúcido com fundo animado.

📱 Totalmente Responsivo: Funciona perfeitamente em Mobile, Tablet e Desktop.

📋 Copiar e Colar Inteligente: Botões dedicados para colar inputs e copiar resultados com feedback visual (Toasts).

🛡️ Validação em Tempo Real: Verifica formatos inválidos e orienta o usuário.

🚀 Zero Dependências de Build: Feito com HTML5 puro e Tailwind via CDN. Basta abrir e usar.

🛠 Tecnologias

HTML5 Semântico: Estrutura da aplicação.

Tailwind CSS (CDN): Estilização, sistema de grid e animações.

JavaScript (Vanilla): Lógica de manipulação de bits e strings.

Lucide Icons: Ícones vetoriais leves e modernos.

Fontes: Inter & JetBrains Mono (Google Fonts).

🚀 Como Usar

Não é necessário instalar node_modules ou rodar servidores de build.

Clone o repositório:

git clone [https://github.com/lyma/eui64-converter.git](https://github.com/lyma/eui64-converter.git)


Abra o arquivo:

Navegue até a pasta e dê um duplo clique em index.html.

O navegador abrirá a ferramenta instantaneamente.

🧠 Lógica EUI-64

Para fins educacionais, veja como a conversão é feita no código:

MAC ➡️ IPv6

Divide o MAC em dois blocos de 24 bits (OUI e NIC Specific).

Insere os bits FFFE (1111 1111 1111 1110) no meio.

Inverte o 7º bit (Universal/Local bit) do primeiro byte.

Adiciona o prefixo fe80::.

IPv6 ➡️ MAC

Verifica se o sufixo contém fffe no meio.

Remove a parte fffe.

Inverte o 7º bit novamente para restaurar o MAC original.

🤝 Contribuição

Contribuições são bem-vindas! Se você tiver ideias para melhorar o design ou a lógica:

Faça um Fork do projeto.

Crie uma Branch (git checkout -b feature/NovaFeature).

Dê commit (git commit -m 'Add: Nova Feature').

Faça o Push (git push origin feature/NovaFeature).

Abra um Pull Request.

📄 Licença

Este projeto está sob a licença MIT. Sinta-se livre para usar e modificar.

<div align="center">
Feito com 💙 e ☕ por <a href="https://github.com/lyma">lyma</a>
</div>
