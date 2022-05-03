ОТВЕТЫ НА ДЗ.


1. commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Jun 18 10:29:58 2020 -0400

    Update CHANGELOG.md
    
    
  каким образом получен результат:   git show aefea



2. v0.12.23

  каким образом получен результат:   git show 85024d3

3. Два  58dcac4b7 ffbcf5581

  каким образом получен результат:   git show b8d720~

4. 
33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24) v0.12.24
b14b74c4939dcab573326f4e3ee2a62e23e12f89 [Website] vmc provider links
3f235065b9347a758efadc92295b540ee0a5e26e Update CHANGELOG.md
6ae64e247b332925b872447e9ce869657281c2bf registry: Fix panic when server is unreachable
5c619ca1baf2e21a155fcdb4c264cc9e24a2a353 website: Remove links to the getting started guide's old location
06275647e2b53d97d4f0a19a0fec11f6d69820b5 Update CHANGELOG.md
d5f9411f5108260320064349b757f55c09bc4b80 command: Fix bug when using terraform login on Windows
4b6d06cc5dcb78af637bbb19c198faff37a066ed Update CHANGELOG.md
dd01a35078f040ca984cdd349f18d0b67e486c35 Update CHANGELOG.md
225466bc3e5f35baa5d07197bbc079345b77525e Cleanup after v0.12.23 release

  каким образом получен результат:   git log v0.12.23..v0.12.24 --pretty=oneline
                                     
                                     
                                     
5. commit 8c928e83589d90a031f811fae52a81be7153e82f
   Author: Martin Atkins <mart@degeneration.co.uk>
   Date:   Thu Apr 2 18:04:39 2020 -0700
   
  каким образом получен результат:  сначала найдены коммиты с функцией func providerSource командой git log -S "func providerSource" --oneline
                                    затем найден нужный коммит git show 8c928e835     
  
6.  8364383c3
    66ebff90c
    41ab0aef7
    52dbf9483
    78b122055
    
   каким образом получен результат: сначала найден файл в котором содержится функция командой git grep  "globalPluginDirs"
                                    затем найдены коммиты фильтрацией по имени файла git log -L:globalPluginDirs:plugins.go --oneline


7.  commit 5ac311e2a91e381e2f52234668b49ba670aa0fe5
Author: Martin Atkins <mart@degeneration.co.uk>
Date:   Wed May 3 16:25:41 2017 -0700
   
   каким образом получен результат: сначала найдены коммиты с упоминанием функции git log -S "func synchronizedWriters"
                                     затем проверены оба коммита git show + кэш выведенных ранее результатов поиска по коммитам.

