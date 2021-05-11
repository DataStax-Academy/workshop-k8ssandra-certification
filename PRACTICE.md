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

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 7.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 8.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 9.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 10.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 11.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 12.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 13.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 14.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)

### Question 15.

<details><summary>Click to view the correct answer</summary>
<p>
    
| The correct answer is ZZZ |
|:---|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip |
</p>
</details>

[⬆️ Top](#sample-questions)


