# prospect-
# Instalations 
...

<!-- @@ à l'installation du projet-->
### A l'installation du projet :
1. création du role Admin : 

        php artisan make:role
        
2. création de user admin et lui assigné le role admin: 

        php artisan make:admin


...
<!-- Gestion des permissions -->
# Restriction sur menu et boutons:
...
1. sur menu :

        @permission('nameOfClass','action')  

        // code

        @endpermission

## Pour le menu, l'action utilisé est read. 

2. sur bouton :

        @permission('nameOfClass','action')  

        // code

        @endpermission

## Liste des actions : 1. read; 2.create; 3. update; 4.delete
...

# Gestion URL
... 

@ Ajouter pour chaque route, le midlleware acces :

        Route::()->middleware('access:nameOfModel');

...
