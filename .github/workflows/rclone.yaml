name: Rclone Bot
on:
  workflow_dispatch:
  schedule:
    - cron:  '59 */5 * * *'
jobs:
  run-sync-service:
    runs-on: ubuntu-latest 
    steps:
      - name: Downloading the Script
        run: |
          wget https://gist.github.com/BlackFoxy616/0e5143fc4c5f1bd2a19c6e69e36999e0/raw/5d538c771821a10037eef8fb550f418e057fd2e2/rclone.sh
      - name: Permission
        run: |
           chmod 777 rclone.sh
      - name: Running the Script
        run: |
           ./rclone.sh
