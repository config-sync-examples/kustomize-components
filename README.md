# kustomize-components

This is a DRY (short for Don't Repeat Yourself) repository, which needs the hydration process to render the WET configs.

It includes a kustomization.yaml file.
The kustomization.yaml file will apply multiple overlays based on the same [base](https://kubectl.docs.kubernetes.io/references/kustomize/glossary/#base).

You can manually run `kustomize` to preview the rendered manifests:
```console
mkdir manifests
kustomize build --output=manifests
```

You can also run `nomos hydrate` to preview the result:
```console
nomos hydrate --output=manifests
```