# Utilizando repositórios com diferentes chave ssh
Passos usados para utilização do github junto ao gitlab que já em execução.

## Ambiente Linux mint

1. [Criar chave](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh) ssh  
`ssh-keygen -t rsa -C “seu email”` 
2. Copiar arquivos id_rsa* criados para pasta  
`/home/"usuario"/.ssh`
3. Adicionar hosts o github no arquivo known_hosts dentro da pasta "/home/user/.ssh"
 `ssh-keyscan github.com >> ~/.ssh/known_hosts`
4. Entrar no github [settings/keys](https://github.com/settings/keys) e adicionar a chave criada
5. Realizar o [clone](https://docs.github.com/pt/repositories/creating-and-managing-repositories/cloning-a-repository) do projeto desejado
