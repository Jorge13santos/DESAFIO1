   ### desafio1
   
       POD=$(kubectl get pods | grep nginx-deploy | awk -F" " '{print $1}')
       
       echo $POD

       kubectl cp desafio.tar $POD:/usr/share/nginx/html
       
    
        kubectl cp index.html $POD:/usr/share/nginx/html
