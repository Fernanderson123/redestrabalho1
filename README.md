# Projeto de Redes de Computadores - Simulação no Packet Tracer

Este repositório contém a simulação de uma rede local desenvolvida para a disciplina de **Redes de Computadores**, ministrada pelo professor **Hermes Pimenta de Moraes Júnior**, na Universidade Federal de Lavras.

## 👥 Alunos

- Anderson Fernandes Barbosa  
- Gabriel Fagundes Mesquita Sousa

## 🗂 Estrutura da Rede

A rede é composta por:

- 4 Hosts (2 PCs e 2 Laptops)
- 3 Servidores físicos distintos
- 1 Switch conectando todos os dispositivos

### Endereçamento IP e Função dos Servidores:

| Nome do Servidor | Função             | Endereço IP      | Nome DNS             |
|------------------|--------------------|------------------|----------------------|
| PAYSANDU         | Servidor Web       | 192.168.1.2      | www.paysandu.com.br  |
| AVAI             | Servidor FTP       | 192.168.1.3      | ftp.avai.com.br      |
| SANTOS           | Servidor DNS       | 192.168.1.4      | dns.santos.com.br    |

### Endereçamento dos Hosts:

| Dispositivo     | IP              |
|-----------------|-----------------|
| PC Luffy        | 192.168.1.10    |
| Laptop Nami     | 192.168.1.11    |
| PC Sanji        | 192.168.1.12    |
| PC Zoro         | 192.168.1.13    |

## 🌐 Servidor Web (PAYSANDU)

O servidor web fornece duas páginas HTML:

- `index.html`: Contém informações da disciplina, professor e alunos.
- `ftp.html`: Lista os usuários e senhas para acesso ao servidor FTP.

### Estrutura dos arquivos HTML:

#### index.html
```html
<h1>Disciplina: Redes de Computadores</h1>
<p>Professor: Hermes Pimenta de Moraes Júnior</p>
<p>Alunos: Anderson Fernandes Barbosa, Gabriel Fagundes Mesquita Sousa</p>
<a href="ftp.html">Acessar informações FTP</a>
```

#### ftp.html
```html
<h1>Usuários e Senhas de acesso do Servidor FTP</h1>
<ul>
  <li>Usuário: aluno1 | Senha: senha123</li>
  <li>Usuário: aluno2 | Senha: abc456</li>
</ul>
<a href="index.html">Voltar para página principal</a>
```

## 📡 Servidor DNS (SANTOS)

O servidor DNS é responsável por resolver os nomes de todos os dispositivos da rede. O domínio utilizado pode ser, por exemplo: rede.local.

Exemplos de nomes configurados:

- www.paysandu.com.br → 192.168.1.2
- ftp.avai.com.br → 192.168.1.3
- dns.santos.com.br → 192.168.1.4

## 📁 Servidor FTP (AVAI)

O servidor FTP está configurado com dois usuários:

| Usuário	| Senha    | 
|---------|----------|
| aluno1	| senha123 |
| aluno2	| abc456   |

## ✅ Requisitos Atendidos

- Quatro hosts configurados e conectados
- Três servidores distintos (Web, FTP, DNS)
- DNS resolvendo nomes locais
- Servidor Web acessível por IP e nome
- Páginas HTML com informações e links
- Servidor FTP com login/senha e troca de arquivos
- Todos os dispositivos conectados via switch
