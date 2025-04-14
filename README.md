# Repositorio APT

Para añadir este repositorio, ejecute:

```bash
# Descargar e instalar la clave GPG
sudo mkdir -p /usr/share/keyrings
wget -qO - https://github.com/SoplosLinux/apt-repo/raw/main/public.key | sudo gpg --dearmor -o /usr/share/keyrings/soplos.gpg

# Añadir el repositorio
echo "deb [signed-by=/usr/share/keyrings/soplos.gpg] https://github.com/SoplosLinux/apt-repo/raw/main stable main" | sudo tee /etc/apt/sources.list.d/soploslinux.list

# Actualizar índices
sudo apt update
```
