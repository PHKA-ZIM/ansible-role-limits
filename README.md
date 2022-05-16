# Limits automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-limits
  name: ansible-role-limits
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-limits

- Import role and override role variables, e.g.
```
- name: Setup limits
  roles:
    - role: ansible-role-limits
```

- All available role vars can be found in `defaults`
