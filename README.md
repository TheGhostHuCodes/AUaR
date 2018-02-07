# Ansible: Up and Running

My workspace containing code listings from the book ["Ansible: Up and
Running"](http://shop.oreilly.com/product/0636920065500.do), by Lorin
Hochstein.

Before trying to run the `playbooks/web-tls.yml` playbook you will need to
generate a TLS certificate and key by executing the following command:

```
openssl req -x509 -nodes -days 3650 -newkey rsa:2048 \
    -subj /CN=localhost \
    -keyout playbooks/files/nginx.key -out playbooks/files/nginx.crt
```
