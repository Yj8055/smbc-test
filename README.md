# smbc-test

apiVersion: argoproj.io/v1alpha1
kind: Application
metadata:
  name: cp4i-apic
spec:
  destination:
    name: ''
    namespace: cp4i-apic
    server: 'https://kubernetes.default.svc'
  source:
    path: overlays/newdv
    repoURL: 'https://github.com/Yj8055/smbc-test.git'
    targetRevision: master
  sources: []
  project: cp4i-apic
  syncPolicy:
    automated: null





API Connect namespace - cp4i-apic
API Connect Cluster CR name - smbc-apic-management
Management subsystem endpoints
cloudManagerEndpoint - cmadmin.apps.o1-773273.cp.fyre.ibm.com
apiManagerEndpoint - apimanager.apps.o1-773273.cp.fyre.ibm.com
platformAPIEndpoint - apiplatform.apps.o1-773273.cp.fyre.ibm.com
consumerAPIEndpoint - consumerapi.apps.o1-773273.cp.fyre.ibm.com
consumerCatalogEndpoint - 
Portal subsystem endpoints
portalAdminEndpoint - api.portal.apps.o1-773273.cp.fyre.ibm.com
portalUIEndpoint - portal.apps.o1-773273.cp.fyre.ibm.com

argocd-sample-argocd-application-controller