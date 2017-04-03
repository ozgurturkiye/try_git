# Digital Ocean sunucuda git in başlatılması ve yerel makinaya clonlanması

1. İlk olarak digitalocean sunucusunda takip edilecek dizin içerisinde `git init` yazılarak git başlatılır.
2. `git add dizin1 dizin2 dosya1 dosya2` yazılarak dosyalar working directoryden, stagin areaya eklenir :)
3. `git commit -m "İlk commmit"` yazılarak değişiklikler depoya commit'lenir. Yani işlenir.
4. `git branch develop` diyerek bir `develop` branch'ı açmakta fayda var :)
5. Şimdi yerel makineye geçilir.
6. Ben clonlamak için ssh kullandım `ssh://[user@]host.xz[:port]/path/to/repo.git/`
7. Uygulaması şu `git clone ssh://username@IPADDRESS/home/ozgur/django_book digitalocean`
8. Sonrası yerel makineden develop branch'a geçilir. `git checkout develop`
9. Değişiklikler yapılıp commitleme işlemi bittikten sonra
10. Yerel makineden `git push origin develop` diyerek bir push edilir.
11. Sonra digitalocean a geçilir.
12. Ve `git merge develop` yazılarak depolar birleştirilir. Hepisi bu kadar şimdilik :)
