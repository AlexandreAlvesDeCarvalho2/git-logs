Um pouco mais sobre git log

Para visualizar pelo CMD o comando (git log --oneline --all --decorate --graph) criei 2 branches e realizei um merge em uma delas.


O Resultado:

![CMD A DOG](https://user-images.githubusercontent.com/58278707/160028887-4d5cf023-6a17-45b3-8b96-9a85852f40e2.PNG)


Algumas formas de utilizar o log

= exibe a lista de commits para o arquivo
      
    git log "filename" 

mostra o histórico a partir de commit_id
      
    git log commit_id  

resume as info de log

    git log --oneline  

resume as infor de log e mostra somente os 4 ultimos log

    git log --oneline -4  

resume as info de log e mostra apartir da data X
  
    git log --oneline --since='2022-03-21' 

resume as info de log e mostra apartir da data X

    git log --oneline --since='2 weeks ago' 

resume as info de log e mostra até a data X

    git log --oneline --until='2022-03-21' 

mostrará todos os logs apartir do 7f526dc até f44fea0
  
    git log --oneline 7f526dc..f44fea0  

mostrará os commits que não estão na branch principal
    
    git log --oneline --all  

mostrará os commits que não estão na branch principal  e indicará de onde é o commit, se é da Branch master ou não

    git log --oneline --all --decorate

o graph irá simbolizar a divisão de Branch exemplo |/ 	
 
    git log --oneline --all --decorate --graph 

outros comandos utilizados

    git branch -a: Lists all the branches
    git branch -d <branch-name>: Deletes the branch in local repo
    git checkout -b: Creates a branch and switches to it
    git checkout <branch-name>: Switches to the provided branch




