## Manual Trigger

## GitHub CLI

```sh
gh workflow run manual_trigger.yml -f message=Hello -f use-emoji=true
```


## Webhook Event
```sh
curl -X POST -H "Accept: application/vnd.github+json" -H "Authorization: token {PAT}" -d '{"event_type": "webhook", client_payload: {"key":"value"} }' https://api.github.com/repos/{owner}/{repo}/dispatches
```