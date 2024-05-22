
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.network "private_network", ip:"192.168.50.41"


  config.vm.provision "shell", inline: <<-SHELL
    sudo apt update     

    sudo apt install mysql-server




  echo "INSERT INTO gestion_clinica_veterinaria.datos_pacientes (IdPaciente, nombre, especie,
  raza, edad, dueño) VALUES" >> /home/vagrant/datos_pacientes.sql

  echo "(1, 'Gabriel', 'Perro', 'Salchicha',3, 'Pedro')," >> /home/vagrant/datos_pacientes.sql
  
  echo "(2, 'Julian', 'Pez', 'Globo',1, 'Pablo')," >> /home/vagrant/datos_pacientes.sql

  
  echo "(3, 'Paco', 'Caballo', 'Arabe',15, 'Santiago');" >> /home/vagrant/datos_pacientes.sql
  
  


  SHELL
 
end
