## Deploy role

Some description for Deploy role would be nice. Any volunteers?

### Parameters

**deploy_ssh_key** (type `string`, default `null`)

Example:
```yaml
deploy_ssh_key: /vagrant/automation/resources/private/id_rsa
```

**deploy_git_repo** (type `string`, default `undefined`)

Example:
```yaml
deploy_git_repo: git@github.com:user/project.git
```

**deploy_git_filemode** (type `bool`, default `true`)

Example:
```yaml
deploy_git_filemode: yes
```

**deploy_git_version** (type `string`, default `HEAD`)

Example:
```yaml
deploy_git_version: v0.0.1
```

**deploy_dest** (type `string`, default `undefined`)

Example:
```yaml
deploy_dest: /var/www/project
```

**deploy_share** (type `array`, default `[]`)

Example:
```yaml
deploy_share:
  - path: app/sessions
    src: sessions
  - path: app/uploads
    src: sessions
```

**deploy_history** (type `int`, default `0`)

Example:
```yaml
deploy_history: 5
```

**deploy_start_hook** (type `string`, default `undefined`)

Example:
```yaml
deploy_start_hook: /vagrant/automation/resources/hooks/deploy.yml
```

**deploy_finish_hook** (type `string`, default `undefined`)

Example:
```yaml
deploy_finish_hook: /vagrant/automation/resources/hooks/deploy.yml
```

**deploy_composer_install** (type `bool`, default `false`)

Example:
```yaml
deploy_composer_install: yes
```

**deploy_npm_install** (type `bool`, default `false`)

Example:
```yaml
deploy_npm_install: yes
```

**deploy_npm_ci** (type `bool`, default `false`)

Example:
```yaml
deploy_npm_ci: yes
```