Ansible Tower config needed

-- Go to users and your username
-- then tokens
-- create token to use in below prometheus config



example Prometheus config

  - job_name: 'tower'
    metrics_path: /api/v2/metrics
    scheme: https
    bearer_token: #generate in Ansible Tower#
    tls_config:
            insecure_skip_verify: true
    static_configs:
            - targets: 
              - #ansible_tower_url#
