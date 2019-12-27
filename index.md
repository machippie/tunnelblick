
## Default Variables

### tunnelblick_enable_automatic_checks

Enable automatic checks

#### Default value

```yaml
tunnelblick_enable_automatic_checks: true
```

### tunnelblick_global_configs

List of global vpn configs

#### Default value

```yaml
tunnelblick_global_configs: []
```

#### Example usage

```yaml
tunnelblick_global_configs:
  - name: Example
    host: vpn.example.com
    port: 1194
    ca: |
      -----BEGIN CERTIFICATE-----
      REDACTED
      -----END CERTIFICATE-----
    crt: |
      -----BEGIN CERTIFICATE-----
      REDACTED
      -----END CERTIFICATE-----
    key: |
      -----BEGIN RSA PRIVATE KEY-----
      REDACTED
      -----END RSA PRIVATE KEY-----
    auth: |
      -----BEGIN OpenVPN Static key V1-----
      REDACTED
      -----END OpenVPN Static key V1-----
```

### tunnelblick_launch_at_next_login

Launch at next login

#### Default value

```yaml
tunnelblick_launch_at_next_login: true
```

### tunnelblick_local_configs

List of global vpn configs

#### Default value

```yaml
tunnelblick_local_configs: []
```

#### Example usage

```yaml
tunnelblick_local_configs:
  - name: Example
    host: vpn.example.com
    port: 1194
    ca: |
      -----BEGIN CERTIFICATE-----
      REDACTED
      -----END CERTIFICATE-----
    crt: |
      -----BEGIN CERTIFICATE-----
      REDACTED
      -----END CERTIFICATE-----
    key: |
      -----BEGIN RSA PRIVATE KEY-----
      REDACTED
      -----END RSA PRIVATE KEY-----
    auth: |
      -----BEGIN OpenVPN Static key V1-----
      REDACTED
      -----END OpenVPN Static key V1-----
```

### tunnelblick_skip_dnsproblem_warning

Skip warning about dns problems

#### Default value

```yaml
tunnelblick_skip_dnsproblem_warning: true
```

### tunnelblick_skip_ipchange_warning

Skip warning that ip address did not change after connection

#### Default value

```yaml
tunnelblick_skip_ipchange_warning: true
```

### tunnelblick_skip_ipnotfetched_warning

Skip warning that ip not fetched before connection

#### Default value

```yaml
tunnelblick_skip_ipnotfetched_warning: true
```

### tunnelblick_started

Start in background after install

#### Default value

```yaml
tunnelblick_started: true
```

### tunnelblick_update_check_automatically

Update check automatically

#### Default value

```yaml
tunnelblick_update_check_automatically: true
```

### tunnelblick_user

User to run user-specific commands

#### Default value

```yaml
tunnelblick_user | default(homebrew_user) | default(ansible_user_id)
```
## Dependencies

None

## License

Apache-2.0

## Author

Thomas Boerger
