# Actions para automatizar o lançamento de versões

É necessário realizar commits, mas a hashtag precisa estar em uma única linha.

# Hashtags disponíveis:

#(release|feat|feature|fix|patch|chore
- \#release: Lançamento de versão, incrementará a versão major do projeto.
- \#feat ou \#feature: Adição de funcionalidade, incrementará a versão minor do projeto.
- \#fix, \#patch: Correção de bug, incrementará a versão patch do projeto.
- \#chore: Alteração de arquivos não relacionados ao funcionamento do projeto. Não incrementará a versão.

# Problemas conhecidos e soluções:

### A action é executada com sucesso, mas não é criada a release e o deploy não é realizado.

- Crie uma primeira release manualmente, no formato `x.y.z`, por exemplo, `0.0.0`.

### Erro "Resource not accessible by integration" ao criar uma release.
- Acesse a página do repositório
- Acesse a aba Settings
- Acesse a seção Actions, no grupo Code and automation
- Clique em General
- Lá em baixo terá a seção Workflow permissions. Selecione Read and Write permissions.
- Salvar.
