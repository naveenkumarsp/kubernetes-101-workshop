# First run

Run the nginx container image

```
$ kubectl run nginx --image nginx

```

And then make it available outside the cluster

```
$ kubectl expose pod nginx --port=80 --target-port=80 --type=NodePort
```
