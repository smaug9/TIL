# notes

## manually run powershell scheduled job

  * 
  
  ```
  (Get-ScheduledJob -id 1).StartJob()
  Receive-Job -id 1
  ```
  
  * ref: https://stackoverflow.com/questions/36691114/powershell-manually-trigger-a-scheduled-job
