# Gerenciamento de Usuários e Permissões (Windows)

## Objetivo

Simular um ambiente corporativo simples para compreender como funciona o controle de acesso a arquivos e pastas utilizando permissões locais no Windows.

O laboratório teve como foco o gerenciamento de usuários, permissões NTFS e restrição de acesso a diretórios sensíveis.

## Ambiente do laboratório

- Sistema Operacional: Windows 11 Home;

- Tipo de rede: LAN doméstica (simulação de ambiente corporativo;

- Computador: Laptop pessoal utilizado para estudos.

## Cenário Simulado

Foi Criado um ambiente fictício representando uma pequena empresa, com diferentes perfis de usuários e níveis de acesso aos diretórios.

## Usuários Criados:

TI_admin

funcionario1

estag

## Estrutura de diretórios

Foi criada uma pasta principal no disco local simulando um servidor de arquivos.

C: Empresa

  -- Compartilhado
  
  -- Restrito

## Descrição das Pastas

Empresa -> Diretório raiz

Compartilhado -> Arquivos acessíveis aos funcionários

Restrito -> Diretório com acesso exclusivo da TI

## Configuração de Permissões

Usuário TI_admin

Possui controle total sobre todas as pastas.

Empresa -> Controle total

Compartilhado -> Controle total

Restrito -> Controle total


Usuário funcionario1

Empresa -> Ler, listar conteúdo e gravar

Compartilhado -> Herdou as permissões da pasta Empresa

Restrito -> Acesso negado


Usuário estag

Empresa -> Leitura e listagem de conteúdo

Compartilhado -> Leitura e listagem de conteúdo

Restrito -> Acesso negado

## Controle de acesso

Para impedir o acesso dos usuários estag e funcionario1 à pasta Restrito, foi utilizada a configuração de negação de pernmissões nas propriedades de segurança da pasta.

Essa configuração garante que apenas o usuário TI_admin tenha acesso ao diretótio restrito.

## Testes realizados

Foram realizados testes de login com cada usuário para validar as permissões configuradas.

## Teste com o funcionario1

- Acesso permitido à pasta Empresa;

- Acesso permitido à pasta Compartilhado;

- Acesso negado à pasta Restrito.

## Teste com o estag

- Acesso permitido à pasta Empresa;

- Acesso permitido à pasta Compartilhado;

- Acesso negado à pasta Restrito.

## Teste com TI_admin 

- Controle total de todas as pastas;

- Capacidade de modificar permissões e criar arquivos.

## Conceitos Aprendidos

- Criação de usuários locais no Windows;

- Configuração de permissões NTFS;

- Controle de acesso a arquivos e diretórios;

- Herança de permissões;

- Restrição de acesso a diretórios sensíveis.

# Conclusão

Este laboratório permitiu compreender na prática como funciona o controle de acesso a arquivos em ambientes Windows.
