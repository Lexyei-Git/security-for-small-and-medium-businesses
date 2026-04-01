# Deployment and Operations

## Recommended SMB approach

OSSEC uses a server-agent model:
- **Server (Manager)**: Central analysis and alerting
- **Agents**: Installed on endpoints to collect data

For SMB:
1. Start with server + 1-3 agents on critical servers
2. Use official source install or packages
3. Configure basic log monitoring and FIM
4. Set up email alerts
5. Expand gradually

## Minimum operational flow (Server)

1. Download source
2. `./install.sh` (choose 'server')
3. Configure `/var/ossec/etc/ossec.conf`
4. `/var/ossec/bin/ossec-control start`
5. Add agents via `/var/ossec/bin/manage_agents`

## Agent installation

1. `./install.sh` (choose 'agent')
2. Extract key from server: `/var/ossec/bin/manage_agents -e <agent_ip>`
3. Import key on agent
4. Restart agent

Official guides:
https://www.ossec.net/docs/docs/manual/installation/install-source.html[web:81]

## Operational cautions

- Server needs reliable uptime and backup
- Agents generate network traffic (logs)
- Test alerts before production
- Start with default rules before customizations
- Monitor server disk usage (logs accumulate)
