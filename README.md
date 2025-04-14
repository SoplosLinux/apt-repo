# Repositorio SoplosLinux

## 🔑 Añadir la clave GPG

```bash
wget -qO - https://raw.githubusercontent.com/SoplosLinux/apt-repo/main/public.key | sudo apt-key add -
```

## 📦 Añadir el repositorio

```bash
echo "deb [signed-by=/usr/share/keyrings/soplos.gpg] https://raw.githubusercontent.com/SoplosLinux/apt-repo/main/ stable main" | sudo tee /etc/apt/sources.list.d/soploslinux.list
```

## 🔄 Actualizar e instalar paquetes

```bash
sudo apt update
sudo apt install nombre-del-paquete
```
