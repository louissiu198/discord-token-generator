# Discord Token Generator

# Cloudfare Requests (cf_bm) [NOT FINISHED]
```py
def generate():
  while True:
    r = requests.get('https://discord.com/cdn-cgi/challenge-platform/h/g/scripts/jsd/19b997cb/invisible.js').text
    try:
      s = r.split("error on cf_chl_props;")[1]
      s = f"0.{s.split("0.")[1]}" 
      try:
          s = s.split(";")[0]
          try:
              s = s.split("/")[0]
              return s
          except:
            return s
      except:
          s = s.split("/;")[0]
          return s
    except:
      continue
  
```
