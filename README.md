# LexGraph Status

Uptime monitor and status page for [LexGraph](https://lexgraph.dev) -- EU AI Act compliance API.

**Live status:** [status.lexgraph.dev](https://status.lexgraph.dev)

## Monitored Endpoints

| Service       | Description                          | Check Interval  |
| ------------- | ------------------------------------ | --------------- |
| API Health    | Liveness check (`/v1/health`)        | Every 5 minutes |
| API Readiness | Dependency health (`/v1/ready`)      | Every 5 minutes |
| Website       | Landing page (`lexgraph.dev`)        | Every 5 minutes |
| API Docs      | Swagger UI (`api.lexgraph.dev/docs`) | Every 5 minutes |

## How It Works

Powered by [Upptime](https://github.com/upptime/upptime) (MIT licensed):

- **GitHub Actions** pings each endpoint on a cron schedule
- **GitHub Issues** are opened automatically when downtime is detected
- **GitHub Pages** serves the public status dashboard
- Uptime history is committed to this repo as version-controlled data

## Configuration

All monitoring configuration is in [`.upptimerc.yml`](./.upptimerc.yml).

## License

- Code: [MIT](./LICENSE) (Upptime framework by [Anand Chowdhary](https://anandchowdhary.com))
- Data in `./history`: [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/)
