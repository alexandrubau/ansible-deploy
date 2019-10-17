## Deploy role

Some description for Deploy role would be nice. Any volunteers?

Inspired by [f500/project_deploy](https://github.com/f500/ansible-project_deploy) role.

### Parameters

**deploy_env** (type `string`, default `dev`)

Example:
```yaml
deploy_env: prod
```

**deploy_dest** (type `string`, default `undefined`)

Example:
```yaml
deploy_dest: /var/www/project
```

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

**deploy_git_version** (type `string`, default `HEAD`)

Example:
```yaml
deploy_git_version: v0.0.1
```

**deploy_git_filemode** (type `bool`, default `true`)

Example:
```yaml
deploy_git_filemode: yes
```

**deploy_pre_build_commands** (type `array`, default `[]`)

Example:
```yaml
deploy_pre_build_commands:
  - /bin/command
```

**deploy_post_build_commands** (type `array`, default `[]`)

Example:
```yaml
deploy_post_build_commands:
  - /bin/command
```

**deploy_environment** (type `object`, default `{}`)

Example:
```yaml
deploy_environment:
  NODE_ENV: production
```

**deploy_unwanted** (type `array`, default `[]`)

Example:
```yaml
deploy_unwanted:
  - app/secret/passwords.txt
```

**deploy_files** (type `array`, default `[]`)

Example:
```yaml
deploy_files:
  - src: app/web/script.js
    dest: app/web/public/script.js
  - src: app/web/script.js
    dest: app/web/public/script.js
    mode: 0777
```

**deploy_templates** (type `array`, default `[]`)

Example:
```yaml
deploy_templates:
  - src: app/env.prod
    dest: app/env
  - src: app/env.local
    dest: app/env
    mode: 0777
```

**deploy_history** (type `int`, default `0`)

Example:
```yaml
deploy_history: 5
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

**deploy_hook_on_initialize** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_initialize: /vagrant/automation/resources/hooks/initialize.yml
```

**deploy_hook_on_update_source** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_update_source: /vagrant/automation/resources/hooks/update-source.yml
```

**deploy_hook_on_create_build_dir** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_create_build_dir: /vagrant/automation/resources/hooks/create-build-dir.yml
```

**deploy_hook_on_build** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_build: /vagrant/automation/resources/hooks/build.yml
```

**deploy_hook_on_make_shared_resources** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_make_shared_resources: /vagrant/automation/resources/hooks/make-shared-resources.yml
```

**deploy_hook_on_finalize** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_finalize: /vagrant/automation/resources/hooks/finalize.yml
```

**deploy_hook_on_complete** (type `string`, default `null`)

Example:
```yaml
deploy_hook_on_complete: /vagrant/automation/resources/hooks/complete.yml
```