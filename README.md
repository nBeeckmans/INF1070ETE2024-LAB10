# INF1070ETE2024-LAB10

## Processus et jobs

Lancer des processus en arrière plan en 1 commande : 

```sh
xeyes & gnome-calculator &
```

Tuer un processus qui est interrompu : 
Le processus n'est pas interrompu. Le processus n'a plus accès a du temps cpu ! Ainsi, le signal de terminaison reçu ne peut pas être géré par le programme. 

## Signaux : 

Suivre les instructions du labo 

## Terminer de force : 

1) tuer a partir d'un autre terminal 

- ouvrir un nouveau terminal 
- `ps aux | grep love `. Prendre le PID. 
- `kill pid` (remplacer le pid par celui trouvé à la commande précédente !)
- `kill -9 %pid` tue le programme ! 

2) fermer le terminal 
3) avec kill : 

Ne marche pas : 
- `CTRL-z` 
- `kill %./love` 
- `fg ./love` 

Marche pas : 
- `CTRL-z` 
- `kill -9 %./love` 
- `fg ./love` 


## Récursivité : 

`pkill fib` ou `killall fib` pour tout tuer. 

| i | nombre de fib | nombre de sleeps |  
|---|---|---|
| 1 | 1 | 1 | 
| 2 | 3 | 3 |
| 3 | 5 | 5 |
| 4 | 9 | 9 | 
| 5 | 15 | 15 |

Patron $ fib i = fib i - 1  + fib i - 2  + 1 $ 

`top` prend le temps de CPU pour ordonner les processus. Cependant, `sleep` ne prend pas de temps de CPU. (voir `time sleep`) 

## Ressources :

Suivez et jouez avec chrome, openoffice, ps, top
