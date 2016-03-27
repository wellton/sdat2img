# sdat2img
Converte uma imagem de dados android (.dat) para imagem com sistema de arquivo ext4 (.img)



## Requisitos
É necessário ter o Python 3.x instalado em seu sistema.

Atualmente suporta Debian (e seus variantes x86/x64), Windows x86/x64 & arquiteturas arm/arm64



## Uso
```
sdat2img.py <transfer_list> <system_new_file> <system_ext4>
```
- `transfer_list` = entrada, system.transfer.list do zip da rom decompactado
- `system_new_file` = entrada, system.new.dat do zip da rom descompactado
- `system_ext4` = saída ext4 do arquivo de imagem



## Exemplo
Este é um exemplo simples em seu sistema Debian (e variantes);
```
~$ ./sdat2img.py system.transfer.list system.new.dat system.img
~$ mkdir imagem
~$ sudo mount -t ext4 -o loop system.img imagem/
```




## Infomação
Para mais informações sobre este binário, visite http://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952.


## Tradução
Traduzido por Wellton Costa de Olivira
www.wellton.com.br
