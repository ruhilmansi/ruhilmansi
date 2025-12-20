<img align="right" width="360" src="https://images.ctfassets.net/wfutmusr1t3h/6eWM76bx8skN2B4Jpvkcil/3ccdafea4229f02802abbd9fc6634a3b/Certifiedtocat_full__2_.svg">

i'm mansi, cs undergraduate at banasthali vidyapith. lately I’m into low level stuff (learning rust) and building things with `<code/>`  sometimes it works, sometimes it doesn’t.

  mail- [mail me ](mailto:mansiruhil@hotmail.com) <br>
  portfolio- [portfolio](https://mansiruhil.vercel.app/) <br>
  linkedin- [linkedin ](https://www.linkedin.com/in/mansi-ruhil-7a00a0228/)
<br>

<br>

![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)
<br>


*my cute lil' hashmap <3 (O(1) always)*

```python
class HashMap:
    def __init__(self):
        self.bucket = []
        for i in range(7):  
            self.bucket.append([])  
        print("hashmap initialized cause built in is too basic")
        # i genuinely love HashMaps <3

    def put(self, key, value):
        index = hash(key) % len(self.bucket)
        for i, (k, v) in enumerate(self.bucket[index]):
            if k == key:
                self.bucket[index][i][1] = value
                print(f" Updated: '{key}' now maps to '{value}'")
                return
        self.bucket[index].append([key, value])
        print(f" Added: '{key}' → '{value}' 'cause i love mapping stuff <3 ")

    def get(self, key):
        index = hash(key) % len(self.bucket)
        for k, v in self.bucket[index]:
            if k == key:
                print(f"Found: '{key}' → '{v}' just like finding answers in life")
                return v
        print(f"Oops: '{key}' not found. doesn’t exist in the map")
        return None

    def remove(self, key):
        index = hash(key) % len(self.bucket)
        before = len(self.bucket[index])
        self.bucket[index] = [pair for pair in self.bucket[index] if pair[0] != key]
        after = len(self.bucket[index])
        if before != after:
            print(f"Removed: '{key}' (if it existed)")
        else:
            print(f"'{key}' wasn’t even here. nothing to remove")

```
<br>
<p align="center"><img src="https://holopin.me/mansiruhil13" alt="cover" /><img loading="lazy" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ruhilmansi&langs_count=100&layout=compact&show_icons=true&include_all_commits=true&count_private=true&custom_title=Programming+Langauges&bg_color=ffffff00&title_color=c9d1d9&border_color=262626&text_color=c9c5c5&border_radius=3" width="100%" alt="Top languages" /><br/></p></a>

<p align="center">
  <iframe src="https://open.spotify.com/embed/track/56sxN1yKg1dgOZXBcAHkJG" width="300" height="80" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
</p>
