# Instructions

Scenario details:

- SR Linux 24.10

Deploy scenario:

```bash
containerlab deploy -t srl01.clab.yml
```

Retrieve YANG Library 1.1 from NETCONF Server:

```bash
docker run -v $(pwd)/netconf:/rpc --rm --network clab -i -t ghcr.io/hellt/netconf-console2:3.0.1 --host clab-srl01-srl --port 830 -u admin -p 'NokiaSrl1!' yang-library/request.xml > netconf/yang-library/reply.xml
```
