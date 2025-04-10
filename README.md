# Distributed Database Node Network
Java-based network of nodes that store key-value data and handle distributed queries using a custom communication protocol.

## Supported operations like:
- `getValue`, `setValue`
- `findKey`, `getMin`, `getMax`
- `newRecord`, `terminateAll`

### 🧾 Compile

```
javac DatabaseNode.java
javac ConnectionThread.java
javac CommunicationHandler.java
javac DatabaseClient.java
```

🚀 Run Node
```
java DatabaseNode -tcpport <TCP_PORT> -record <key>:<value> [ -connect <host>:<port> ]
```

🧑‍💻 Run Client
```
java DatabaseClient -gateway <host>:<TCP_PORT> -operation <operation_with_parameters>
```
