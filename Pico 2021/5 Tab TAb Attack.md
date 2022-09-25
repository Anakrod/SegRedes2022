# Nombre del reto
### Tab TAb Attack
## Objetivo
```
Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/72712e82413e78cc8aa8d553ffea42b0/Addadshashanammu.zip)
HINT: After `unzip`ing, this problem can be solved with 11 button-presses...(mostly Tab)...
```
## Solucion
``` shell 
┌──(anitars㉿kali)-[~/Descargas]
└─$ unzip Addadshashanammu.zip 
Archive:  Addadshashanammu.zip
   creating: Addadshashanammu/
   creating: Addadshashanammu/Almurbalarammi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/
  inflating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet  
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      file  ltdis.sh                  static   warm
Addadshashanammu.zip  flag  Obsidian-0.15.9.AppImage  strings  warm.1
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ cd Addadshashanammu 
                                                                             
┌──(anitars㉿kali)-[~/Descargas/Addadshashanammu]
└─$ ls
Almurbalarammi
                                                                             
┌──(anitars㉿kali)-[~/Descargas/Addadshashanammu]
└─$ cd Almurbalarammi  
                                                                             
┌──(anitars㉿kali)-[~/Descargas/Addadshashanammu/Almurbalarammi]
└─$ ls               
Ashalmimilkala
                                                                             
┌──(anitars㉿kali)-[~/Descargas/Addadshashanammu/Almurbalarammi]
└─$ cd Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku 
                                                                             
┌──(anitars㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ ls 
fang-of-haynekhtnamet
                                                                             
┌──(anitars㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ cat fang-of-haynekhtnamet 
 HH/lib64/ld-linux-x86-64.so.2GNUGNU� �"!�▒@����a       ~���= 
                                                              Y h "libc.so.6puts__cxa_finalize__libc_start_mainGLIBC_2.2.5_ITM_deregisterTMCloneTable__gmo � � � � � � H�H��sterTMCloneTableu▒i   1�
 H��t��H���5�
 �%�
 @�%�
 h������%�
H�=�����^H��H���PTL��H�
 �DH�=�
 UH��
 H9�H��tH�Z
]��f.�]�@f.�H�=i
 H�5b
 UH)�H��H��H��H��?H�H��t▒H�!
 H��t
     ]��f�]�@f.��=
8#TT 1tt$D���o�N
�� ��0)@▒�    H�(;▒�                                                                             ��t 1��L��L��D��A��H��H9�u�H�[]A\A]A^A_Ðf.���H�H��*ZAP!* 
┌──(anitars㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ strings fang-of-haynekhtnamet 
/lib64/ld-linux-x86-64.so.2
libc.so.6
puts
__cxa_finalize
__libc_start_main
GLIBC_2.2.5
_ITM_deregisterTMCloneTable
__gmon_start__
_ITM_registerTMCloneTable
AWAVI
AUATL
[]A\A]A^A_
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_6f332f10}
;*3$"
GCC: (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
crtstuff.c
deregister_tm_clones
__do_global_dtors_aux
completed.7698
__do_global_dtors_aux_fini_array_entry
frame_dummy
__frame_dummy_init_array_entry
fang-of-haynekhtnamet.c
__FRAME_END__
__init_array_end
_DYNAMIC
__init_array_start
__GNU_EH_FRAME_HDR
_GLOBAL_OFFSET_TABLE_
__libc_csu_fini
_ITM_deregisterTMCloneTable
puts@@GLIBC_2.2.5
_edata
__libc_start_main@@GLIBC_2.2.5
__data_start
__gmon_start__
__dso_handle
_IO_stdin_used
__libc_csu_init
__bss_start
main
__TMC_END__
_ITM_registerTMCloneTable
__cxa_finalize@@GLIBC_2.2.5
.symtab
.strtab
.shstrtab
.interp
.note.ABI-tag
.note.gnu.build-id
.gnu.hash
.dynsym
.dynstr
.gnu.version
.gnu.version_r
.rela.dyn
.rela.plt
.init
.plt.got
.text
.fini
.rodata
.eh_frame_hdr
.eh_frame
.init_array
.fini_array
.dynamic
.data
.bss
.comment
                                                                             
┌──(anitars㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ strings fang-of-haynekhtnamet | grep pico
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_6f332f10}


Descomprimimos el archivo que descargamos, vamos viendo que tiene y entrando a los archivos, despues de ver, hacemos un cd y damos tabulador hasta que nos indique que es todo el directorio, entramos y leemos lo que hay en el archivo, como no esta legible, aplicamos un strings, al estar la bandera escondida entre tanto texto, aplicamos un grep para encontrarla de inmediato.
```
## Referencias
