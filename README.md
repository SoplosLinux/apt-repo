# Repositorio SoplosLinux 📦

Repositorio de paquetes .deb para Soplos Linux.

## ✨ Características

- Paquetes oficiales de Soplos Linux
- Actualizaciones automáticas vía APT
- Firma GPG para mayor seguridad
- Soporte para todas las versiones

## 🚀 Instalación

Para añadir este repositorio sigue estos sencillos pasos:

### 1. Añadir la clave GPG

```bash
# Descargar e instalar la clave GPG
sudo mkdir -p /usr/share/keyrings
wget -qO - https://github.com/SoplosLinux/apt-repo/raw/main/public.key | sudo gpg --dearmor -o /usr/share/keyrings/soplos.gpg
```

### 2. Añadir el repositorio

```bash
# Añadir el repositorio
echo "deb [signed-by=/usr/share/keyrings/soplos.gpg] https://github.com/SoplosLinux/apt-repo/raw/main/ stable main" | sudo tee /etc/apt/sources.list.d/soploslinux.list

# Actualizar índices
sudo apt update
```

### 3. Instalar paquetes

```bash
sudo apt install nombre-del-paquete
```

## 🔍 Buscar paquetes disponibles

Puedes ver la lista de paquetes disponibles con:

```bash
apt search soplos
```

## 📝 Licencia

Este repositorio y sus paquetes están licenciados bajo GPL-3.0

## 🤝 Soporte

Si tienes problemas o preguntas:
- 🌐 Web: https://soplos.org
- 📧 Email: info@soplos.org
- 💬 Foro: https://foro.soplos.org
