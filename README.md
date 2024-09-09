# Zuul demo repository!
Added new parameter....!
check..
..
...
...
.
zookeeper-servers:
  - host: zk
    port: 2281
zookeeper-tls:
  cert: /var/certs/certs/client.pem
  key: /var/certs/keys/clientkey.pem
  ca: /var/certs/certs/cacert.pem

labels:
  - name: ubuntu-jammy

providers:
  - name: static-rack
    driver: static
    pools:
      - name: main
        nodes:
          - name: 10.0.2.15
            labels: ubuntu-jammy
            timeout: 13
            host-key: ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIPnoo1JeMSmciQp3mILctSmm3A+tQaVExaIiPruq9VYr
            username: barath
....
.
