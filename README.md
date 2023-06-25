# Discord Token Generator

# Cloudfare Requests (cf_bm) [NOT FINISHED] [s Param]
I did this below 2 minutes so dont blame code, just it works
```py
def generate():
    while True:
        r = requests.get('https://discord.com/cdn-cgi/challenge-platform/h/g/scripts/jsd/19b997cb/invisible.js').text
        try:
            s = r.split("error on cf_chl_props;")[1]
            s = f"0.{s.split('0.')[1]}" 
            try:
                s = s.split(";")[0]
                try:
                    s = s.split("/")[0]
                    try:
                        s = s.split("'.split('")[0]
                        return s
                    except:
                        return s
                except:
                    return s
            except:
                s = s.split("/;")[0]
                return s
        except:
            continue
while True:
    print(generate())
```
