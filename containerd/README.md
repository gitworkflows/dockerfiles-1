# containerd

```console
$ docker run -dit --name containerd --user nobody docker-pkg/containerd
$ docker exec -it containerd bash
nobody@828358e6a99a:/$ ctr content fetch --all-platforms ghcr.io/foo/bar:baz
...
nobody@828358e6a99a:/$ ctr images push --user jsmith ghcr.io/baz/bar:foo ghcr.io/foo/bar:baz
...
```
