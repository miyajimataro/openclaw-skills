# Google Calendar Skill (via gog)

## description
Googleカレンダーの予定確認と予定作成を行うスキル

## commands

### create_event
予定を作成する（予定追加・スケジュール登録など

```bash
gog calendar create primary \
  --summary "{{summary}}" \
  --from "{{from}}" \
  --to "{{to}}"

```


### list_events
予定を確認する（今日の予定・スケジュール確認など）

```bash
gog calendar events list primary \
  --from "$(date +%Y-%m-%d)T00:00:00+09:00" \
  --to "$(date +%Y-%m-%d)T23:59:59+09:00"

```
