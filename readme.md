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

**deploy_version** (type `string`, default `HEAD`)

Example:
```yaml
deploy_version: v0.0.1
```

**deploy_dest** (type `string`, default `undefined`)

Example:
```yaml
deploy_dest: /var/www/project
```

**deploy_override** (type `bool`, default `false`)

Example:
```yaml
deploy_override: yes
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

**deploy_composer_path** (type `string`, default `undefined`)

Example:
```yaml
deploy_composer_path: /vagrant/composer.json
```

**deploy_npm_path** (type `string`, default `undefined`)

Example:
```yaml
deploy_npm_path: /vagrant/package.json
```

**deploy_npm_ci** (type `bool`, default `false`)

Example:
```yaml
deploy_npm_ci: yes
```