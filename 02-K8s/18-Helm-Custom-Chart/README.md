 469  mkdir 17-Helm
  470  cd 17-Helm/
  471  ls
  472  vim helm-rbac.yaml
  473  kubectl create -f helm-rbac.yaml
  474  helm repo add azure-marketplace https://marketplace.azurecr.io/helm/v1/repo
  475  helm search repo nginx
  476  helm install my-release azure-marketplace/nginx
  477  helm list
  478  kubectl  get pods
  479  helm install my-nginx azure-marketplace/nginx
  480  helm list
  481  kubectl  get pods
  482  kubectl  get svc
  483  ls
  484  vim README.md
  485  ls
  486  cd ..
  487  ls
  488  mkdir 18-Helm-Custom-Chart
  489  ls
  490  cd 18-Helm-Custom-Chart/
  491  helm create sample-chart
  492  ls
  493  cd sample-chart/
  494  ls
  495  ls -R .
  496  ls
  497  cat templates/deployment.yaml
  498  ls
  499  vim values.yaml
  500  ls
  501  cd ..
  502  ls
  503  helm install my-sample-app sample-chart --dry-run
  504  helm install my-sample-app sample-chart
  505  helm list
  506  kubectl  get pods
  507  kubectl  get pods,svc
  508  ls
  509  helm list
  510  helm uninstall my-sample-app
  511  helm uninstall my-release
  512  helm uninstall my-nginx
  513  helm list
  514  ls
  515  helm create my-py-app
  516  ls
  517  cd my-py-app/
  518  ls
  519  vim values.yaml
  520  vim templates/deployment.yaml
  521  ls
  522  cd ..
  523  ls
  524  helm install mypyapp my-py-app --dry-run
  525  helm install mypyapp my-py-app
  526  helm  list
  527  kubectl  get pods
  528  kubectl  get svc
