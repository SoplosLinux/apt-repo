# 📦 Repositorio SoplosLinux APT

Repositorio oficial de paquetes para SoplosLinux.

## ⚡ Características

- 🔒 Paquetes firmados con GPG
- 🔄 Actualizaciones automáticas vía APT
- 🚀 Alto rendimiento y velocidad
- 💻 Compatibilidad total con Debian/Ubuntu

## 🛠️ Instalación

### 1️⃣ Añadir la clave GPG

```bash
# Descargar e instalar la clave GPG
sudo mkdir -p /usr/share/keyrings
wget -qO - https://github.com/SoplosLinux/apt-repo/raw/main/public.key | sudo gpg --dearmor -o /usr/share/keyrings/apt-repo.gpg
```

### 2️⃣ Añadir el repositorio

```bash
# Añadir la fuente APT
echo "deb [signed-by=/usr/share/keyrings/apt-repo.gpg] https://github.com/SoplosLinux/apt-repo/raw/main/ stable main" | sudo tee /etc/apt/sources.list.d/soploslinux.list

# Actualizar índices
sudo apt update
```

### 3️⃣ Instalar paquetes

```bash
sudo apt install nombre-del-paquete
```

## 🔍 Buscar paquetes disponibles

Para ver todos los paquetes disponibles:

```bash
apt search soplos
```

## 🤝 Contribuir

¿Encontraste un error o tienes una sugerencia? ¡Abre un issue!

## 📝 Licencia

Este repositorio está bajo la licencia GPL-3.0.
