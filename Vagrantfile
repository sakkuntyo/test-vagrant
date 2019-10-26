Vagrant.configure("2") do |config|
  config.vm.box = "antonilin/mint-19-mate"

  # 設定を変更しないとＵＳＢ2.0をオフにしろと言われるので、オフにする
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--usb", "off"]
    vb.customize ["modifyvm", :id, "--usbehci", "off"]
  end
end
