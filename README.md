# PoC

```sh
rpmseclint [spec file]
```

The spec file must have a `VCS:` tag with the following structure:

```
git+[GIT REPO URL]#[TAG]
```

And `Source0:` must be the tar containing the source represented in the git repo.

For example:

```
VCS: git+https://git.kernel.org/pub/scm/libs/%{name}/%{name}.git#%{name}-%{version}
Source0: https://mirrors.edge.kernel.org/pub/linux/libs/security/linux-privs/libcap2/%{name}-%{version}.tar.gz
```

