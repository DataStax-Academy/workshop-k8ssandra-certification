## 🎓🔥 K8ssandra Certification Workshop 🔥🎓

[![License Apache2](https://img.shields.io/hexpm/l/plug.svg)](http://www.apache.org/licenses/LICENSE-2.0)
[![Discord](https://img.shields.io/discord/685554030159593522)](https://discord.com/widget?id=685554030159593522&theme=dark)

This section will run you through a set of practice exam questions.  These practice exam questions are also available as a sample exam in the interface used for the *real* certification exams at [https://tests.mettl.com/authenticateKey/32m7zxbyf4](https://tests.mettl.com/authenticateKey/32m7zxbyf4).

[<-- Back to MAIN](./README.md)

## Sample Questions

### Question 1.
Which is a valid statement about security in a Cassandra cluster named `cluster1`, created with the Cass Operator?

**A.** The Cass Operator will not enable security in the cluster.

**B.** The Cass Operator will create a superuser with username: `cassandra`.

**C.** The Cass Operator will create a superuser with username: `cluster1-superuser`.

**D.** The Cass Operator will create a superuser based on credentials defined in the yaml file.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is C |
|:---|
| The Cass Operator creates a secure Cassandra cluster. Unlike a local Cassandra installation, the super user will be: `cluster1-superuser`. The password for this user will be stored in a Kubernetes secret. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 2.

Which two are required to create a cluster with the Cass Operator? (Choose two)

**A.** a datacenter name

**B.** a storage class

**C.** a keystore

**D.** a rack name

**E.** a cluster name

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answers are B and E |
|:---|
| All Cassandra clusters must have a cluster name. Since Cassandra is a database, it must be stateful. Therefore the Cass Operator requires a k8s storage class. Datacenters, racks and keystores are optional in Cassandra. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 3.
Which two are valid statements about containers running in the same Kubernetes Pod? (Choose two)

**A.** Containers in a Pod always run in different hardware or virtual machines.

**B.** Containers in a Pod always share network resources.

**C.** Containers in a Pod always run in the same hardware or virtual machine.

**D.** Containers in a Pod always run the same application.

**E.** Containers in a Pod always expose ports outside the Kubernetes cluster.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answers are B and C |
|:---|
| A Pod may house multiple containers. Containers in a Pod share network resources and run on the same hardware or virtual machine.

Containers in the same Pod often run different applications. Containers may offer services that are only used in the K8s cluster and do not need to be exposed to the outside world.
|
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 4.

Which two Kubernetes operators are included in K8ssandra? (Choose 2)

**A.** cass-operator

**B.** reaper-operator

**C.** stargate-operator

**D.** docker-operator

**E.** helm-operator

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answers are A and B |
|:---|
| K8ssandra includes the cass-operator and reaper-operator. There is no stargate-operator.  Docker and Helm are not included in the K8ssandra deployment and there are no Docker or Helm operators. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 5.

Which three are features of Medusa? (Choose three)
 
**A.** scheduled backups

**B.** single node backup

**C.** differential backups

**D.** cluster wide backup

**E.** single node restore

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answers are B, C and D |
|:---|
| Medusa supports single node backup and restore including differential backups. Medusa does not have scheduling capability -- external tools like cron can provide rudimentary scheduling features. Likewise, Medusa instances backup individual Cassandra nodes. Medusa does not perform *cluster-wide* backups. To do *cluster-wide* backup,  set up an external orchestration tool to manage Medusa instances. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 6.

Which Docker commands create a Docker network and run Cassandra in a container using that network?

**A.** `docker network create d-net`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`docker run --network d-net cassandra`

**B.** `docker network start d-net`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`docker run --network d-net cassandra`

**C.** `docker network create d-net`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`docker run d-net cassandra`
       
**D.** `docker network start d-net`   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`docker run d-net cassandra`

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is A |
|:---|
| Create a Docker network with the `docker network create` command and use the `--network` switch when running the container to use the named network.|
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 7.

How do clients authenticate to the Stargate Auth API using Table-based authentication/authorization?

**A.** username and password

**B.** two-way SSL/TLS

**C.** SAML token
 
**D.** JWT

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is A |
|:---|
| Table-based authentication and authorization uses the Stargate Auth API to generate an auth token based on a Cassandra username and password. The auth-table-based-service uses the generated auth token to allow Stargate API queries access to the Cassandra data. JWT-based authentication and authorization is an *alternative* to Table-based authentication and authorization. Stargate does not support authentication through two-way SSL/TLS or SAML.
 |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 8.

How does Prometheus communicate with Cassandra?

**A.** JMX

**B.** SNMP

**C.** TLS

**D.** UDP

<details><summary>Click to view the correct answer</summary>
<p>
   
| The correct answer is A |
|:---|
| Java Management Extensions (JMX) is the native management protocol for Java applications and the JVM. Prometheus uses JMX to monitor Cassandra. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 9.

Given that a Docker container named `Main01` was started with the journald logging driver, which Docker command can be used to view its logs?

**A.** `docker logs -f Main01`

**B.** `docker cat -f logs --name Main01`

**C.** `docker logs --name Main01`

**D.** `docker cat -f Main01`

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is A |
|:---|
| The command `docker logs -f <container-name>`  displays log files for a container. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 10.

Which two commands can re-start a stopped Docker container named NodeZ? (Choose two.)

**A.** `docker run NodeZ`

**B.** `docker restart NodeZ`

**C.** `docker resume NodeZ`

**D.** `docker start NodeZ`

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answers are B and D |
|:---|
| The commands `docker restart` and `docker start` can *re-start* a stopped container. `docker run` creates a new container and there is no `docker resume` command. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 11.

Which is an advantage of using Reaper over nodetool to perform repairs?

**A.** Reaper can do incremental repairs.

**B.**  Reaper can do full repairs.

**C.**  Reaper can repair data when nodes are down.

**D.**  Reaper can schedule repairs.


<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is D |
|:---|
| Reaper and nodetool can both initiate incremental and full repairs. Neither tool can do a repair on a downed node. A big advantage of Reaper is that it can schedule repairs. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 12.

Which tool installs K8ssandra?

**A.** RPM

**B.**  YUM

**C.**  Helm

**D.**  apt-get

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is C |
|:---|
| K8ssandra is a Kubernetes application so it is installed using a Helm chart. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 13.

Consider the following service manifest:

```
kind: Service
apiVersion: v1
metadata:
  name: my-service
spec:
  selector:
    app: my-app
  ports:
    - protocol: TCP
      port: 80
      targetPort: 8080
```
Which is a valid statement about `my-service`?

**A** The service makes `my-app` available outside the Kubernetes cluster on port 80.

**B** The service makes `my-app` available outside the Kubernetes cluster on port 8080.

**C** The service makes `my-app` available inside the Kubernetes cluster on port 80.

**D** The service makes `my-app` available inside the Kubernetes cluster on port 8080.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is C |
|:---|
| This service manifest exposes `my-app` outside the cluster. The internal port is 8080 and the external port is 80. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 14.

In K8ssandra, how does Grafana collect Cassandra metrics.

**A.** Grafana connects directly to Cassandra.

**B.** Grafana gets Cassandra metrics from Medusa.

**C.** Grafana gets Cassandra metrics from Reaper.

**D.** Grafana gets Cassandra metrics from Prometheus.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is D |
|:---|
| Prometheus is the K8ssandra component that monitors Cassandra. Grafana gets metrics from Prometheus. |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 15.

Given the output from this command: (You may need to scroll left/right to see the entire output.)

```
% kubectl get pods
NAME                                           READY STATUS   RESTARTS AGE
some-really-really-long-meaningless-pod-name-0 2/2   Running  0        2m34s
some-really-really-long-meaningless-pod-name-1 0/2   Running  0        2m34s
some-really-really-long-meaningless-pod-name-2 1/2   Running  0        2m34s
```

Which is a valid statement about `some-really-really-long-meaningless-pod-name-2`?

**A.** The pod and all its containers are running.

**B.** The pod and one of its containers are running.

**C.** The pod and its container are in stage 1 of the initialization process.

**D.** The pod is running and its container is in stage 1 of the initialization process.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is B |
|:---|
| In this example the pod’s status is `Running`. Looking at the Ready column, the pod has two containers and one is ready (running.) |
</p>
</details>

[⬆️ Top](#sample-questions)


