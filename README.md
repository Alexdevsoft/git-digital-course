# Curso Digital: git

## Salvando alterações no repositório

- comando git push
- comando git pull
- comando git fetch

O comando git push é utilizado para enviar as alterações feitas em um repositório local para um repositório remoto. Isso geralmente ocorre após a realização de commits locais. O comando básico é:

git push [nome-do-repositório-remoto] [nome-do-branch]

Por exemplo, para enviar as alterações do branch master para o repositório remoto chamado origin, você usaria:

git push origin master

Esse comando atualiza o repositório remoto com os commits que estão no branch local, permitindo que outros colaboradores vejam suas alterações.
git pull
O comando git pull combina duas operações: ele busca (fetch) as alterações do repositório remoto e, em seguida, mescla (merge) essas alterações no branch atual do repositório local. O comando é frequentemente usado para atualizar seu branch local com as últimas mudanças feitas por outros colaboradores. O uso básico é:

git pull [nome-do-repositório-remoto] [nome-do-branch]

Por exemplo:

git pull origin master

Esse comando traz as alterações do branch master do repositório remoto origin e as mescla automaticamente no seu branch local. Se houver conflitos entre as alterações locais e remotas, o Git solicitará que você resolva esses conflitos antes de concluir a mesclagem134.
git fetch
O comando git fetch é utilizado para baixar as referências e commits de um repositório remoto sem mesclá-los automaticamente no branch atual. Isso permite que você veja quais alterações estão disponíveis antes de decidir integrá-las ao seu trabalho. O uso básico é:

git fetch [nome-do-repositório-remoto]

Por exemplo:

git fetch origin

Após executar esse comando, você pode verificar as alterações baixadas usando git log ou git diff, mas seu branch local permanecerá inalterado até que você decida mesclar essas mudanças manualmente123.
Diferenças entre os Comandos
git push: Envia suas alterações locais para o repositório remoto.
git pull: Baixa e mescla as alterações do repositório remoto no seu branch atual.
git fetch: Baixa as alterações do repositório remoto, mas não altera seu branch atual até que você decida fazer isso.
Esses comandos são fundamentais para o trabalho colaborativo em projetos que utilizam o Git, permitindo uma gestão eficiente das versões e das contribuições de diferentes desenvolvedores
