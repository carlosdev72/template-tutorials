# Plantilla para realizar tutoriales con gitbook
Plantilla que sirve para realizar tutoriales y publicarlos en github.com

Aqui tienes información de como duplicar un repositorio  

https://help.github.com/articles/duplicating-a-repository/

1. Creamos un repositorio en GitHub  


2. Creamos un clon limpio de ese repositorio en una carpeta local temporal.
  
    `git clone --bare https://github.com/carlosdev72/template-tutorials.git`

3. Desde la carpeta local temporal subimos el codigo al repositorio creado en GitHub  

    `cd template-tutorials.git`  
    `git push --mirror https://github.com/useraccount/new-repository.git`  

4. Eliminamos la carpeta temporal local  
`cd ..`
`rm -rf old-repository.git`

Alternativamente, también puede simplemente descargar un archivo comprimido de este repositorio y luego usar los 
comandos estándar para inicializar y subir a su nuevo repositorio.  

```bash
git init
git add .
git commit -m"first commit"
git remote add origin git@github.com:useraccount/new-repository.git  
git push origin master
```



