   ### desafio1
   
       Executando um deploy com volume nfs - Digital-Ocean
       
     ### 01. 
        Instalando NFS-SERVER no SERVIDOR ( pode ser um node ou nfs-server )
        # apt-get install nfs-server -y 
        # mkdir -p /srv/nfs/data
        # chmod -R 777 /srv/nf
        # Adicione esse diretório no arquivo /etc/exports  com as devidas permissões.
         /srv/nfs/data    *(rw,sync,no_subtree_check,insecure)
        # exportfs -a ( verifcação de status nfs) 
        # showmount -e ( validação do compartilhamento)
       
      ###02
        # apt install nfs-common -y   ( instalando client do nfs nos nodes do cluster)
        
        # showmount -e (ip nfs-server)
        # showmount -e ip-nfs-server mount -t nfs ip-nfs-server:/srv/nfs/data /root/data 
        # mount | grep data
        
        ###03
         # 
        
        
        
        
        
       
       
      
