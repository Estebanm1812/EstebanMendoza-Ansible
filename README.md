# Ansible
En este repositorio se explicaran los pasos para ejecutar un Contenedor Con Super Mario Infinite usando terraform, Azure y ansible
### Primer Paso
Tener la infraestructura para una Maquina Virtual en Azure con Ip Publica y Acceso por SSH con usuario y Contrasena
### Segundo Paso
Clonar este Repositorio que tiene la gestion del Asinble, Modificando la informacion del Host a la propia y elegiendo un puerto al cual respondera el servicio
### Tercer Paso
Ejecutar los Siguientes Comandos:
ansible-playbook -i inventory/hosts.ini playbooks/install_docker.yml
ansible-playbook -i inventory/hosts.ini playbooks/run_container.yml
Adicionalmente hay que dar permisos al folder del proyecto, para esto se puede usar el siguiente comando:
chmod 777 EstebanMendoza-Ansible
### Cuarto Paso
Por medio de la interfaz de Azure hay que realizar una nueva regla de Red, de tipo entrada en la que se habilite el puerto elegido al inicio


### Evidencias Del Playbook Install Docker
<img width="1014" alt="Captura de pantalla 2024-04-09 a la(s) 9 11 20 p  m" src="https://github.com/Estebanm1812/EstebanMendoza-Ansible/assets/69942961/50543d5e-6125-417f-aee6-db640e269dfb">
### Evidencias Del Playbook Run Container
<img width="1014" alt="Captura de pantalla 2024-04-09 a la(s) 9 11 45 p  m" src="https://github.com/Estebanm1812/EstebanMendoza-Ansible/assets/69942961/cfd8b890-e99f-4070-8f11-45051be1583c">
### PortForwading

<img width="1155" alt="Captura de pantalla 2024-04-09 a la(s) 9 14 07 p  m" src="https://github.com/Estebanm1812/EstebanMendoza-Ansible/assets/69942961/b599c9f2-4973-4e83-8c79-c5279f542cd0">
### Evidencias del Juego de Mario Funcionando
<img width="1155" alt="Captura de pantalla 2024-04-09 a la(s) 9 14 30 p  m" src="https://github.com/Estebanm1812/EstebanMendoza-Ansible/assets/69942961/f26de23e-d9e9-44b2-8afc-122da9974b15">
