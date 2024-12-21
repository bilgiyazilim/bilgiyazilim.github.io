# Bilgi Yazılım Topluluğu Websitesi

[![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=for-the-badge&logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)

[bilgiyazilim.github.io](https://bilgiyazilim.github.io) websitesinin içerikleri ve
konfigürasyonları.

## Deployments

main branch'e yapılan her commit (dolayısıyla da merge) sonrası [Deploy to GitHub
Pages](https://github.com/bilgiyazilim/bilgiyazilim.github.io/blob/main/.github/workflows/github-pages.yml)
workflow'u otomatik olarak tetiklenir. Bu workflow, main branch içerisinde websitenin build'ini alıp
github pages üzerinden yayına alır.

Yani [bilgiyazilim.github.io](https://bilgiyazilim.github.io) sitesinin güncellenmesi için yapılması
gereken tek şey değişikliğin main branch'e aktarılmasıdır. Gerisini hazırlanan workflow
halledecektir.

## Siteyi Yerelinde Ayağa Kaldır

> Yerelinizde python3 kurulu olması gerekmektedir.

Repoyu yereline clone'la:
```
$ git clone https://github.com/bilgiyazilim/bilgiyazilim.github.io.git
```

Proje klasörüne geç:
```
$ cd bilgiyazilim.github.io
```

İhtiyaç duyulan Python paketlerinin yerelinizdeki Python paketlerini bozmaması için virtual
environment oluştur ve aktif et:
```
$ virtualenv venv
$ source venv/bin/activate
```

İhtiyaç duyulan Python paketlerini kur:
```
(venv) $ pip install -r requirements.txt
```

Websiteyi ayağa kaldır:
```
(venv) $ make serve
```

> Yerelinizde `make` komutu mevcut değilse `$ mkdocs serve -w overrides/` komutunu kullanabilirsiniz

Bu komut sonrasında site `http://localhost:8000` adresinde ayağa kalkacaktır. Eğer site ayağa
kalkmadıysa veya komut sonrası bir hata mesajı aldıysanız Discord üzerinden yardım istemekten
çekinmeyin.