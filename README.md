# kubernetes
Kubernetes AWS Fixes

# Fix AWS Logging
cd /tmp;
wget https://raw.githubusercontent.com/morissette/kubernetes/master/fluentd-es.yaml
cp -v /tmp/fluentd-es.yaml /etc/kubernetes/manifests/fluentd-es.yaml 
cp -v /tmp/fluentd-es.yaml /srv/salt/fluentd-es/fluentd-es.yaml 
cp -v /tmp/fluentd-es.yaml /usr/share/google/kubernetes/saltbase/salt/fluentd-es/fluentd-es.yaml
rm -vf /tmp/fluentd-es.yaml
