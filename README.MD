This project can be built manually with `docker build -f ci/Dockerfile workdir`.

I would expect the app spec to look like:
```
services:
- name: web
  root_path: workdir
  dockerfile_path: ci/Dockerfile
```
