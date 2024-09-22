# Git&GitHub Master Guide
Esta es una guía paso a paso para aprender a usar *Git* y *GitHub*.

## 1. Configurar Git por primera vez
Lo primero que debes hacer es configurar tu nombre de usuario y correo electrónico global en Git. Este correo es el que se asociará con tus commits en cualquier proyecto.
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@example.com"
```

Puedes verificar tu configuración con:
```bash
git config --global --list

```
> [!NOTE]
> Para ejecutar esta linea de código se requiere *less* cómo dependencia, si no lo tienes instalado ejecuta:
```bash
# Para una distribución Debian o derivados.
sudo apt-get install less
```

## 2. Inicializar un nuevo repositorio

Ahora que Git está configurado, puedes inicializar un repositorio:
1. Crea una carpeta o navega a la carpeta que quieras convertir en un repositorio:
```bash
mkdir nombre-del-proyecto
cd nombre-del-proyecto
```
2. Inicializa el repositorio Git en esa carpeta:
```bash
git init
```
*Esto crea un repositorio vacío*

## 3. Añadir archivos al repositorio
Una vez que tienes archivos en tu proyecto, puedes agregar archivos al área de preparación (staging area) antes de confirmarlos (commit):
1. Crea o añade archivos en tu directorio.
2. Verifica el estado de los archivos no rastrados
```bash
git status
```
3. Añade los archivos al área de preparación:
```bash
git add archivo.txt
```
O para añadir todos los archivos
```bash
git add .
```

## 4. Hacer un commit
Una vez que los archivos están en el área de preparación, haz un commit para guardar los cambios:
```bash
git commit -m "Mensaje del commit"
```

## 5. Conectar el repositorio local a GitHub
