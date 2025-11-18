# INSTRUCCIONES PARA SUBIR EL PROYECTO A GITHUB

## Paso 1: Crear Cuenta en GitHub (si no tienes)
1. Ve a https://github.com
2. Click en "Sign up"
3. Completa el registro con tu email
4. Verifica tu email

## Paso 2: Crear Nuevo Repositorio
1. Click en el botón "+" en la esquina superior derecha
2. Selecciona "New repository"
3. Nombre del repositorio: `club-america`
4. Descripción: "Sitio web informativo del Club América - Proyecto Escolar"
5. Selecciona "Public"
6. NO marques "Initialize this repository with a README"
7. Click en "Create repository"

## Paso 3: Instalar Git (si no lo tienes)

### Windows
1. Descarga Git desde: https://git-scm.com/download/win
2. Ejecuta el instalador
3. Usa las opciones por defecto

### Mac
```bash
# Instalar Homebrew primero (si no lo tienes)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Instalar Git
brew install git
```

### Linux
```bash
sudo apt-get update
sudo apt-get install git
```

## Paso 4: Configurar Git (Primera vez)
```bash
# Configurar tu nombre
git config --global user.name "Tu Nombre"

# Configurar tu email (el mismo de GitHub)
git config --global user.email "tu-email@ejemplo.com"

# Verificar configuración
git config --list
```

## Paso 5: Inicializar Repositorio Local
```bash
# Navegar a la carpeta de tu proyecto
cd ruta/a/tu/proyecto/club-america

# Inicializar Git
git init

# Verificar que se creó la carpeta .git
ls -la
```

## Paso 6: Agregar Archivos al Repositorio
```bash
# Ver estado de archivos
git status

# Agregar todos los archivos
git add .

# O agregar archivos específicos
git add index.html
git add jugadores.html
git add historia.html
git add contacto.html
git add cs.css
git add README.md
git add .gitignore

# Verificar archivos agregados
git status
```

## Paso 7: Hacer el Primer Commit
```bash
# Crear commit con mensaje descriptivo
git commit -m "Proyecto inicial: Sitio web Club América"

# Verificar commit
git log
```

## Paso 8: Conectar con GitHub
```bash
# Agregar repositorio remoto (reemplaza [tu-usuario] con tu usuario de GitHub)
git remote add origin https://github.com/[tu-usuario]/club-america.git

# Verificar conexión
git remote -v
```

## Paso 9: Subir Archivos a GitHub
```bash
# Subir archivos a la rama main
git push -u origin main

# Si te pide autenticación, usa tu usuario y contraseña de GitHub
# O mejor aún, usa un Personal Access Token
```

## Paso 10: Configurar GitHub Pages
1. Ve a tu repositorio en GitHub
2. Click en "Settings"
3. En el menú lateral, click en "Pages"
4. En "Source", selecciona "Deploy from a branch"
5. En "Branch", selecciona "main" y "/" (root)
6. Click en "Save"
7. Espera 1-5 minutos
8. Tu sitio estará disponible en: `https://[tu-usuario].github.io/club-america/`

## Comandos Git Útiles para el Futuro

### Ver cambios
```bash
git status              # Ver archivos modificados
git diff               # Ver diferencias en archivos
git log                # Ver historial de commits
```

### Hacer cambios
```bash
git add archivo.html   # Agregar archivo específico
git add .              # Agregar todos los archivos
git commit -m "mensaje" # Crear commit
git push               # Subir cambios a GitHub
```

### Actualizar desde GitHub
```bash
git pull               # Descargar cambios de GitHub
```

### Crear ramas (para trabajo avanzado)
```bash
git branch nueva-rama  # Crear nueva rama
git checkout nueva-rama # Cambiar a nueva rama
git merge nueva-rama   # Fusionar rama
```

## Solución de Problemas Comunes

### Error: "fatal: not a git repository"
```bash
# Asegúrate de estar en la carpeta correcta
cd ruta/a/tu/proyecto
git init
```

### Error: "remote origin already exists"
```bash
# Eliminar remote existente
git remote remove origin

# Agregar nuevamente
git remote add origin https://github.com/[tu-usuario]/club-america.git
```

### Error: "failed to push some refs"
```bash
# Hacer pull primero
git pull origin main --allow-unrelated-histories

# Luego push
git push origin main
```

### Autenticación con Personal Access Token
1. Ve a GitHub Settings
2. Developer settings
3. Personal access tokens
4. Generate new token
5. Selecciona permisos: repo
6. Copia el token
7. Úsalo como contraseña cuando Git te lo pida

## Verificación Final

### Checklist
- [ ] Repositorio creado en GitHub
- [ ] Git instalado y configurado
- [ ] Archivos subidos correctamente
- [ ] README.md visible en GitHub
- [ ] GitHub Pages configurado
- [ ] Sitio accesible en la URL de GitHub Pages

### URLs Importantes
- Repositorio: `https://github.com/[tu-usuario]/club-america`
- Sitio web: `https://[tu-usuario].github.io/club-america/`

## Recursos Adicionales
- Documentación Git: https://git-scm.com/doc
- GitHub Guides: https://guides.github.com/
- GitHub Pages: https://pages.github.com/
- Tutorial Git: https://www.atlassian.com/git/tutorials

---

**¡Felicidades!** Tu proyecto ya está en GitHub y publicado en internet.
