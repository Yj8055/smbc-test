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
