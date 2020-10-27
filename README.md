<img src="https://camo.githubusercontent.com/992babdffd8c74a1502de375fbdf7e4d54773242/68747470733a2f2f6d656469612e67697068792e636f6d2f6d656469612f53576f536b4e36447854737a71494b4571762f67697068792e676966" width="89%">

---
<p align="center">
<a href="mailto:dimasyudha@domainm.my.id" target="_blank"><img alt="Gmail" src="https://img.shields.io/badge/-Gmail-c14438?style=flat&logo=Gmail&logoColor=white"></a>
<a href="https://www.instagram.com/dimasydha" target="_blank"><img alt="Instagram" src="https://img.shields.io/badge/-Instagram-C13584?style=flat&logo=Instagram&logoColor=white"></a>
<a href="https://www.linkedin.com/in/dimasyudha" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/-LinkedIn-0072b1?style=flat&logo=Linkedin&logoColor=white"></a>
<a href="https://t.me/dimasyudha" target="_blank"><img alt="Telegram" src="https://img.shields.io/badge/-Telegram-0088CC?style=flat&logo=Telegram&logoColor=white"></a>
<a href="https://twitter.com/intent/follow?screen_name=dmsydha" target="_blank"><img alt="Twitter" src="https://img.shields.io/badge/-Twitter-00acee?style=flat&logo=Twitter&logoColor=white"></a>
<a href="https://www.youtube.com/UC6f6Jv1QqDgxOtJYRciTHoA/playlists" target="_blank"><img alt="YouTube" src="https://img.shields.io/badge/-YouTube-FF0000?style=flat&logo=YouTube&logoColor=white"></a>
</p>

---
```python3

from dataclasses import dataclass
from typing import Tuple


class Meta(type):
    def __new__(cls, name, bases, attrs):
        for attr in attrs:
            if not attr.startswith("_"):
                __annotations__[attr] = Tuple[str, ...]
        attrs["__annotations__"] = __annotations__
        new_cls = super().__new__(cls, name, bases, attrs)
        new_cls = dataclass(new_cls)
        return new_cls


class Stack(metaclass=Meta):
    languages   = ("C", "Java", "Python")
    ongoing     = ("Kotlin", "React Native")


print("about me")

dimasyudha = {
    'fullname': 'Dimas Yudha Pratama',
    'othername': ['Dimas', 'Yudha', 'Tama'],
    'nationality': ['Indonesia'],
    'location': 'Kediri, East Java',
    'contact': {
        'email': 'dimasyudha@domainm.my.id',
        'website': 'https://www.dimasyudha.com',
    },
    'about': [
        'Graduated English language college student',
        'Have a keen interest in all things tech',
        'Currently working on Android stuffs',
        'An Android maintainer for MI 8 SE device',
        'Love live open source'
    ],
    'motto': ['Reach your feature bright bridge by doing not talking']
}
```
<p align="center">
  <a href="https://andyruwruw.vercel.app/api/now-playing?open">
    <img src="https://andyruwruw.vercel.app/api/now-playing">
  </a>
</p>

<p align="center">
  <img src="https://andyruwruw.vercel.app/api/top-played">
</p>