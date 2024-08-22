# kubernetes-csi
实现对接kubernetes 和ceph的对接， 使用社区提供的`csi` https://github.com/ceph/ceph-csi/tree/devel
解决在部署时遇到的坑。
只需要修改
```bash
csi-config-map.yaml
csi-rbd-secret.yaml
csi-rbd-sc.yaml
```
中的认证信息和`clusterID`即可。
最后`kubectl apply -f .`
参考文档
https://docs.ceph.com/en/reef/rbd/rbd-kubernetes/
