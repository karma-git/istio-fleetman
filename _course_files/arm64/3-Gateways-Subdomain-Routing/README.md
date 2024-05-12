```
k apply -f .
k port-forward -n istio-system svc/istio-ingressgateway 8080:80
<!-- k port-forward -n istio-system svc/istio-ingressgateway 8080:80 -->

while true;
  do curl -H "Host: fleetman.com" http://localhost:8080/api/vehicles/driver/City%20Truck ; 
  sleep 1.5;
  echo "\n";
done

btw: разницы если что не видно :(
```
