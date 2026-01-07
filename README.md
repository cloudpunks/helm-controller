# helm-controller

This repository defines a [Kustomize][kustomize] manifest which could be used by
other repositories to generate a [Kubernetes][kubernetes] manifest for the
installation of [helm-controller][project].

## Usage

```yaml
---
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization
namespace: kube-system

resources:
  - github.com/cloudpunks/helm-controller?ref=v1.1.12

...
```

## Security

If you find a security issue please contact ops@cloudpunks.de first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

* [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```
Copyright (c) 2023 cloudpunks GmbH <info@cloudpunks.de>
```

[kustomize]: https://kustomize.io/
[kubernetes]: https://kubernetes.io/
[project]: https://github.com/k3s-io/helm-controller
