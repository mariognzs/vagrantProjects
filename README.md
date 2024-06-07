```markdown
# Vagrant Projects

Este repositorio contiene archivos y scripts para la configuración y gestión de múltiples entornos de máquinas virtuales utilizando Vagrant.

## Descripción de los Archivos

- **vagrant-vms/**: Directorio que contiene diferentes `Vagrantfile` para varias configuraciones de máquinas virtuales.
- **shellscripts/**: Directorio con scripts de shell utilizados para el provisionamiento y configuración de las máquinas virtuales.
- **.gitignore**: Archivo para excluir archivos y directorios específicos del control de versiones.

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalados los siguientes programas en tu sistema:

- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Instrucciones de Uso

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/mariognzs/vagrantProjects.git
   cd vagrantProjects/vagrant-vms
   ```

2. **Seleccionar y configurar el entorno deseado:**
   
   Dirígete al subdirectorio que contiene el `Vagrantfile` para la configuración específica que deseas usar, por ejemplo:

   ```bash
   cd ubuntu-setup
   ```

3. **Iniciar la máquina virtual:**

   Ejecuta el siguiente comando dentro del directorio del `Vagrantfile` seleccionado:

   ```bash
   vagrant up
   ```

   Este comando descargará la caja base especificada (si aún no está en tu sistema), creará y configurará la máquina virtual según las instrucciones definidas.

4. **Acceder a la máquina virtual:**

   Una vez que la máquina virtual esté en funcionamiento, puedes acceder a ella mediante SSH:

   ```bash
   vagrant ssh
   ```

5. **Detener la máquina virtual:**

   Para detener la máquina virtual, usa el comando:

   ```bash
   vagrant halt
   ```

6. **Destruir la máquina virtual:**

   Si ya no necesitas la máquina virtual y deseas liberar espacio en disco, puedes destruirla con el siguiente comando:

   ```bash
   vagrant destroy
   ```

## Personalización

Puedes personalizar la configuración de las máquinas virtuales editando los `Vagrantfile` en los subdirectorios correspondientes. Consulta la [documentación oficial de Vagrant](https://www.vagrantup.com/docs) para más detalles sobre las opciones de configuración disponibles.
