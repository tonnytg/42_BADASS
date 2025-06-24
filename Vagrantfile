Vagrant.configure("2") do |config|
  # Usa a box Ubuntu Desktop 22.04 para Intel (x86_64)
  config.vm.box = "peru/ubuntu-22.04-desktop-amd64"

  # Nome da VM
  config.vm.hostname = "ubuntu-desktop"

  # Aloca mais recursos (ajuste conforme necessário)
  config.vm.provider "virtualbox" do |vb|
    vb.name = "UbuntuDesktop2204"
    vb.memory = 4096
    vb.cpus = 2
  end

  # Encaminha a interface gráfica (GUI)
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
  end

  # Porta para acesso remoto (opcional)
  config.vm.network "forwarded_port", guest: 22, host: 2222, id: "ssh"

  # Provisão básica (pode remover se não quiser)
  config.vm.provision "shell", inline: <<-SHELL
    echo "Sistema iniciado com Ubuntu Desktop 22.04"
    sudo apt-get update -y
    sudo apt-get upgrade -y
  SHELL
end
