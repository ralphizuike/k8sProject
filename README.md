# etech-k8sproject1
mysql-webapp deployment
Steps to follow:
step1: deploy your mysql database
#use the kubectl utility tool

step2: Deploy the mysql service pod

step3: deploy your wordapp container pod

step4: deploy your wordapp service and expose the application

Exercise:
1. Create your username and password on the wordapp 
2. Access the mysql pod and show the database


1  sudo hostnamectl set-hostname KubeMaster
    2  sudo su - ubuntu
    3  ls
    4  kubectl get nodes
    5  ls -a
    6  cd .kube/
    7  ls
    8  cat config
    9  cd
   10  kubectl get nodes
   11  kubectl get nodes -o json | jq
   12  kubectl get ns
   13  kubectl get pods -n kube-system
   14  kubectl describe pod kube-apiserver-kubemaster -n kube-system
   15  kubectl get pods -n kube-system
   16  kubectl describe pod kube-controller-manager-kubemaster -n kube-system
   17  kubectl get pods -n kube-system
   18  kubectl describe pod kube-scheduler-kubemaster -n kube-system
   19  kubectl get pods -n kube-system
   20  kubectl describe pod etcd-kubemaster -n kube-system
   21  kubectl get pods -n kube-system
   22  kubectl logs -f kube-apiserver-kubemaster -n kube-system
   23  kubectl config get-contexts
   24  kubectl config use-contexts kubernetes-admin@kubernetes
   25  kubectl config use-context kubernetes-admin@kubernetes
   26  kubectl config view
   27  kubeadm upgrade plan
   28  sudo kubeadm upgrade plan
   29  kubectl -n kube-system get cm kubeadm-config -o yaml
   30  kubectl explain pod
   31  sudo vi pod.yaml
   32  ls
   33  kubectl apply -f pod.yaml
   34  kubectl get pods
   35  kubectl describe pod etech-app
   36  kubectl get pod -o wide
   37  sudo vi profile
   38  ls4
   39  ls
   40  cat pod.yaml
   41  kubectl get nodes
   42  kubectl get pods
   43  kubectl describe pod etech-app
   44  kubectl pod -o wide
   45  kubectl get pod -o wide
   46  kubectl get pod -o json | jq
   47  ls
   48  sudo vi podsvc.yaml
   49  kubectl apply -f podsvc.yaml
   50  kubectl get svc
   51  cat podsvc.yaml
   52  kubectl get svc
   53  kubectl describe svc etechapp-service
   54  kubectl get pods
   55  kubectl get rs
   56  kubectl delete rs frontend
   57  kubectl get pods
   58  kubectl get pods -o wide
   59  kubectl delete etech-app
   60  kubectl delete pod etech-app
   61  ls
   62  kubectl get ns
   63  kubectl create ns riike
   64  kubectl kubectl get ns riike -o yaml
   65  kubectl get ns riike -o yaml
   66  kubectl get ns riike -o yaml > miike.yaml
   67  ls
   68  sudo vi miike.yaml
   69  cat miike.yaml
   70  kubectl apply -f miike.yaml
   71  kubectl get ns
   72  kubectl get ns miike -o yaml
   73  kubectl get ns
   74  sudo vi deployriike.yaml
   75  ls
   76  kubectl apply -f deployriike.yaml
   77  sudo vi deployriike.yaml
   78  kubectl apply -f deployriike.yaml
   79  sudo vi deployriike.yaml
   80  cat -n deployriike.yaml
   81  ls
   82  rm -f deployriike.yaml
   83  ls
   84  sudo vi deployriike.yaml
   85  kubectl apply -f deployriike.yaml
   86  kubectl get deploy
   87  sudo vi deployriike.yaml
   88  kubectl get deploy -n riike
   89  kubectl get pods -n riike
   90  kubectl edith deploy myapp-deployment -n riike
   91  kubectl edit deploy myapp-deployment -n riike
   92  kubectl get pods -n riike
   93  kubectl get deploy -n riikesvc.yaml [B
   94  kubectl get pods -n riike
   95  kubectl describe pod myapp-deployment-bcb686658-c78f7 -n riike
   96  kubectl get pods -n riike
   97  kubectl logs -f myapp-deployment-bcb686658-c78f7 -n riike
   98  kubectl logs -f myapp-deployment-59bc6649ff-c4zcn -n riike
   99  kubectl rollout history deploy myapp-deployment -n riike
  100  kubectl rollout undo deploy myapp-deployment -n riike
  101  kubectl get pods -n riike
  102  kubectl edit deploy myapp-deployment -n riike
  103  kubectl get svc -n riike
  104  kubectl get pod -n riike
  105  kubectl exec -ti myapp-deployment-59bc6649ff-c4zcn -n riike -- /bin/bash
  106  kubectl exec -it myapp-deployment-59bc6649ff-c4zcn -n riike -- /bin/bash
  107  ls
  108  sudo rm -f deployriike.yaml
  109  sudo vi deployriike.yaml
  110  kubectl apply -f deployriike.yaml
  111  kubectl get ns
  112  kubectl get deploy
  113  kubectl get deploy riike
  114  kubectl get deploy -o wode riike
  115  kubectl get deploy -n riike
  116  kubectl get pods -n riike
  117  sudo vi riikesvc.yaml
  118  ls
  119  sudo vi riikesvc.yaml
  120  ls
  121  kubectl apply -f riikesvc.yaml
  122  kubectl get svc
  123  kubectl get svc -n riike
  124  kubectl get svc -n riike -o json | jq
  125  kubectl get svc -n riike
  126  kubectl describe svc myapp-deployment-svc -n riike
  127  kubectl edit svc myapp-deployment-svc -n riike
  128  kubectl get deploy -n riike
  129  kubectl scale deploy myapp-deployment -n makeup --replicas=10
  130  kubectl scale deploy myapp-deployment -n riike --replicas=10
  131  kubectl get deploy -n riike
  132  kubectl describe svc myapp-deployment-svc -n riike
  133  kubectl get pods -n riike
  134  kubectl scale deploy myapp-deployment -n riike --replicas=3
  135  kubectl get pods -n riike
  136  kubectl get rs -n riike
  137  kubectl edit deploy myapp-deployment -n riike
  138  ls
  139  kubectl get svc -n riike
  140  kubectl delete svc myapp-deployment-svc -n riike
  141  kubectl get svc -n riike
  142  kubectl get pods -n riike
  143  kubectl create ns vivian
  144  kubectl get ns vivian
  145  kubectl get ns
  146  ls
  147  kubectl apply -f riikesvc.yaml
  148  kubectl get ns
  149  kubectl get ns riike
  150  kubectl get svc -n riike
  151  kubectl describe svc myapp-deployment-svc -n riike
  152  kubectl get svc -n riike
  153  kubectl delete svc myapp-deployment-svc -n riike
  154  kubectl delete svc myapp-deployment-svc -n vivian
  155  kubectl get deploye -n riike
  156  kubectl get deploy -n riike
  157  kubectl delete deploy myapp-deployment -n riike
  158  kubectl get deploy -n riike
  159  git clone https://github.com/ralphizuike/k8sProject.git
  160  ls
  161  cd k8sProject/
  162  ls
  163  cat README.md
  164  cat mysql-service.yaml
  165  ls
  166  cat mysqlnew.yaml
  167  ls
  168  cat wordpod.yaml
  169  ls
  170  cat wordsvc.yaml
  171  kubectl apply -f mysqlnew.yaml
  172  kubectl apply -f mysql-service.yaml
  173  kubectl describe svc mysql-service.yaml
  174  kubectl describe svc mysql-service
  175  ls
  176  kubectl apply -f wordpod.yaml
  177  kubectl apply -f wordsvc.yaml
  178  kubectl get rs -n riike
  179  kubectl get pods
  180  history
  181  kubectl get deploy
  182  kubectl get svc
  183  kubectl get pods
  184  kubectl -it mysql-deployment-db6c6cc9c-hd2jk
  185  kubectl -it mysql-deployment-db6c6cc9c-hd2jk -- /bin/bash
  186  kubectl exec -it mysql-deployment-db6c6cc9c-hd2jk -- /bin/bash
  187  history
  188  kubectl exec -it mysql-deployment-db6c6cc9c-hd2jk -- /bin/bash
  189  ls
  190  kubectl get deploy
  191  kubectl get pods
  192  kubectl get svc
  193  kubectl describe svc mysql-service
  194  kubectl describe svc wordpress-service
  195  history
  196  kubectl exec -it mysql-deployment-db6c6cc9c-hd2jk -- /bin/bash
  197  history
  198  kubectl get pods
  199  kubectl get deploy
  200  history
  201  kubectl get pods
  202  kubectl exec -it wordpress-deployment-7f7d997455-7bhnv -- /bin/bash
  203  history
  204  kubectl get svc
  205  kubectl get svc
  206  kubectl get pods
  207  kubectl exec -ti wordpress-deployment-7f7d997455-7bhnv -- /bin/bash
  208  ls
  209  kubectl get node
  210  kubectl get nodes
  211  sudo apt-get install nfs-common
  212  kubectl get nodes
  213  kubectl get pods
  214  echo -n "raphael" | base64
  215  history
  216  echo -n "raphael" | base64
  217  echo -n
  218  echo -n "cmFwaGFlbA==" | base64 -d
  219  kubectl get secret
  220  kubectl get secret -o json | jq
  221  kubectl get secret -n kube=system
  222  kubectl get secret -n kube-system
  223  echo -n "raphael" | base64
  224  sudo vi secrettest.yaml
  225  kubectl apply -f secrettest.yaml
  226  kubectl get secret
  227  echo -n "vivian" | base64
  228  sudo vi secret2.yaml
  229  kubectl apply -f secret2.yaml
  230  kubectl get secret
  231  kubectl describe secret mysql-iketech
  232  kubectl get ns
  233  ls
  234  sudo vi secret2.yaml
  235  kubectl apply -f secret2.yaml
  236  kubectl get secret -n riike
  237  kubrctl get secret -n riike -o yaml
  238  kubectl get secret -n riike -o yaml
  239  kubectl delete secret --all
  240  kubectl get secret
  241  kubectl delete secret -n riike --all
  242  sudo vi pv.yaml
  243  kubectl apply -f pv.yaml
  244  kubectl get pv
  245  kubectl get pv -o yaml
  246  sudo vi pvc.yaml
  247  kubectl apply -f pvc.yaml
  248  kubectl get pv -o yaml
  249  kubectl get pv
  250  kubectl get pvc
  251  kubectl describe pvc myclaim
  252  kubectl delete pvc --all
  253  kubectl get pv
  254  kubectl delete pv --all
  255  kubectl get pv
  256  sudo vi storage.yaml
  257  kubectl apply -f storage.yaml
  258  kubectl get storageclass
  259  kubectl get storageclass -o json | jq
  260  sudo vi secret.yaml
  261  kubectl apply -f secret.yaml
  262  sudo vi pv-wordpress-mysql.yaml
  263  kubectl apply -f pv-wordpress-mysql.yaml
  264  kubectl get pv
  265  sudo vi pvc-wordpress.yaml
  266  kubectl apply -f pvc-wordpress.yaml
  267  sudo vi pvc-mysql.yaml
  268  kubectl apply -f pvc-mysql.yml
  269  kubectl apply -f pvc-mysql.yaml
  270  kubesctl get pv
  271  kubectl get pv
  272  sudo vi svc-deploy-mysql.yaml
  273  kubectl apply -f svc-deploy-mysql.yaml
  274  sudo vi svc-deploy-mysql.yaml
  275  kubectl apply -f svc-deploy-mysql.yaml
  276  sudo vi svc-deploy-wordpress.yaml
  277  kubectl apple -f svc-deploy-wordpress.yaml
  278  kubectl apply -f svc-deploy-wordpress.yaml
  279  kubectl get svc
  280  kubectl get deployment
  281  kubectl get pods
  282  kubectl describe pod wordpress-859fbdcd8f-965d9 -o json | jq
  283  kubectl get pod  -o json | jq
  284  kubectl get svc
  285  kubectl get pods
  286  kubectl get ns
  287  kubectl create ns etechvault
  288  kubectl get ns
  289  cat ./config
  290  cat .kube/config
  291  sudo kubectl config set-context --current --namespace etechvault
  292  cat .kube/config
  293  cat .kube/config | grep namespace
  294  export VERIFY_CHECKSUM=false
  295  curl https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 | bash
  296  helm version
  297  helm repo add hashicorp https://helm.releases.hashicorp.com
  298  helm install vault --set='ui.enabled=true' --set='ui.serviceType=NodePort' --set='server.dataStorage.enabled=false' hashicorp/vault --version 0.16.1
  299  kubectl get pods
  300  kubectl get svn
  301  kubectl get svc
  302  kubectl get pods
  303  kubectl exec -it vault-0 -- /bin/sh
  304  kubectl create serviceaccount app
  305  kubectl exec -it vault-0 -- /bin/sh
  306  kubectl describe clusterrolebinding vault-server-binding
  307  kubectl get pods
  308  kubectl get svc
  309  ls
  310  cat secret.yaml
  311  kubectl get pods
  312  sudo vi .kube/config
  313  kubectl get pods
  314  kubectl get pod -n etechvault
  315  kubectl delete pod vault-0 -n etechvault
  316  kubectl delete pod vault-agent-injector-6cc6f46c6c-ttppc -n etechvault
  317  kubectl get svc -n etechvault
  318  kubectl delete svc --all -n etechvault
  319  kubectl get svc -n etechvault
  320  helm uninstall vault
  321  helm uninstall vault -n etechvault
  322  kubectl delete ns etechvault
  323  ls
  324  history
ubuntu@KubeMaster:~$
