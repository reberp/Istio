## Terms

service mesh
* Containers think they're talking to services, but actually talking to proxies on pods that injected logic to route traffic
* gives you the ability to have insight into inter-pod comm easily
Data plane - basically just a plane that represents all the proxy containers
Control plane - basically just istiod, or the things controlling istio proxies. Can also have Kiali and others. 

## About

How it routes
* containers on pods in the istio-system NS
* old version with pilot, etc. new version simplified and put them all into istiod
* pods call istiod to give it info on what is happening and then send call to other proxy 

istiod
* 

## How to implement

Shouldn't have to make any changes to containers. Can switch on/off ideally. Tracing is an exception.

