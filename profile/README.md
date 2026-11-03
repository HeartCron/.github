# Heartcron

[Heartcron](https://heartcron.com) watches cron jobs, scheduled tasks and websites,
and alerts you by email, Telegram, Slack, Discord or webhook when something
doesn't run on time, fails or goes down.

Add one request to the end of a job:

```sh
0 3 * * * /opt/backup.sh && curl -fsS https://ping.heartcron.com/<check-uuid>
```

or wrap it with the CLI, which also reports the exit code, duration and output:

```sh
0 3 * * * heartcron run nightly-backup -- /opt/backup.sh
```

## Open source

| Repository | What it is |
|---|---|
| [cli](https://github.com/HeartCron/cli) | `heartcron run`, `ping` and `checks` for Linux, macOS and Windows |
| [ping-action](https://github.com/HeartCron/ping-action) | GitHub Action that reports scheduled workflow runs |
| [examples](https://github.com/HeartCron/examples) | Ready setups for Bash, Docker, Kubernetes, systemd, Laravel, Python and Node |

## Links

[Website](https://heartcron.com) · [Docs](https://heartcron.com/docs/) · [Guides](https://heartcron.com/guides/) · [Cron expression tool](https://heartcron.com/cron/) · hello@heartcron.com
