# DataVizBusqueda
# 1. Inicializa git si no lo has hecho
git init

# 2. Agrega todos los archivos
git add .

# 3. Guarda los cambios
git commit -m "Preparando despliegue para DataVizBusqueda"

# 4. Asegura que estás en la rama main
git branch -M main

# 5. Conecta con TU repositorio específico (si ya existe un origin, usa 'set-url' en vez de 'add')
git remote remove origin 2> /dev/null
git remote add origin https://github.com/federicaham/DataVizBusqueda.git

# 6. Sube el código (te pedirá tus credenciales de GitHub si no las tienes configuradas)
git push -u origin main --force
