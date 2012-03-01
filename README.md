* rename de directory abiquo_upgrade_1.8.5-HF7 using the current release name

* put binary RPMs in abiquo_upgrade_1.8.5-HFX directory

* use createrepo inside abiquo_upgrade_1.8.5-HFX

    cd abiquo_upgrade_1.8.5-HFX && createrepo -s sha -d .

* tweak install.sh.in changing ABI_VERSION and SUPPORTED_VERSION
  values

* create a tarball from abiquo_upgrade_1.8.5-HFX

  tar czf abiquo_upgrade_1.8.5-HFX.tar.gz abiquo_upgrade_1.8.5-HFX

* run  make-installer.sh
    
    make-installer.sh abiquo_upgrade_1.8.5_HFX.tar.gz

* rename install.sh to whatever you want

    mv install.sh abiquo_upgrade_1.8.5-HFX.bin
