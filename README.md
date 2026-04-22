# Guía Rápida: Instalación y Uso de NVM (Node Version Manager)

Esta guía te permitirá gestionar múltiples versiones de **Node.js** de forma sencilla en tu sistema.

---

## 1. Instalación de NVM

En linux. Ejecuta el script de instalación oficial desde la terminal:

```bash
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

En Windows [Descargar NVM para Windows](https://github.com/coreybutler/nvm-windows/releases)
Ejecutá nvm-setup.exe

## 2. Refrescar la Configuración

Para que la terminal reconozca los cambios sin tener que cerrarla, carga el archivo de configuración de tu shell:

```bash
source ~/.bashrc
```

O cerrá y abrí la terminal (CMD o PowerShell)

## 3. Verificar Instalación

Comprueba que NVM esté correctamente instalado:

```bash
nvm --version
```
> Debe devolver un número de versión (ej. `0.39.7`).

---

## 4. Gestión de Versiones de Node.js

### Instalar la versión estable (LTS)
```bash
nvm install --lts
```

### Configurar versión por defecto
Para que se active automáticamente al abrir una terminal:
```bash
nvm alias default 'lts/*'
```

### Instalar una versión específica
Por ejemplo, la versión 20:
```bash
nvm install 20
```

### Cambiar entre versiones
Para correr wollok por ejemplo
```bash
nvm use 20
```

---

## Comandos Útiles

| Comando | Descripción |
| :--- | :--- |
| `nvm ls` | Ver versiones instaladas localmente. |
| `nvm ls-remote` | Ver todas las versiones disponibles para instalar. |
| `nvm current` | Ver qué versión estás usando ahora. |
| `node -v` | Confirmar la versión de Node activa. |

---
