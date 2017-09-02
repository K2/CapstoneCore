# CapstoneCore
CoreCLR 64bit Capstone bindings

```ps
PS /mnt/hgfs/inVteroCore/master/inVtero.net/inVtero.core/inVteroCore/bin/Release/netstandard2.0> $Bytes = [Byte[]] @( 0x90, 0xcc, 0x10, 0xf1, 0x10, 0xe7, 0x11, 0xf2, 0x31, 0xe7, 0xdc, 0xa1, 0x2e, 0xf3, 0xe8, 0x4e, 0x62, 0xf3 )                                                                        
PS /mnt/hgfs/inVteroCore/master/inVtero.net/inVtero.core/inVteroCore/bin/Release/netstandard2.0> uname -a                                            
Linux ubuntu 4.10.0-32-generic #36~16.04.1-Ubuntu SMP Wed Aug 9 09:19:02 UTC 2017 x86_64 x86_64 x86_64 GNU/Linux
PS /mnt/hgfs/inVteroCore/master/inVtero.net/inVtero.core/inVteroCore/bin/Release/netstandard2.0> Get-CapstoneDissassembly -D 0 -Bytes $Bytes                                                                                                                                                              
Done
insn                                                            detail                         
----                                                            ------                         
0x0 [1] nop  ; 0x90 0x9c 0x52 0x7f                              CapstoneCore.Capstone+cs_detail
0x1 [1] int3  ; 0xcc 0x0 0x0 0x0                                CapstoneCore.Capstone+cs_detail
0x2 [2] adc cl, dh ; 0x10 0xf1 0x0 0x0                          CapstoneCore.Capstone+cs_detail
0x4 [2] adc bh, ah ; 0x10 0xe7 0x0 0x0                          CapstoneCore.Capstone+cs_detail
0x6 [2] adc edx, esi ; 0x11 0xf2 0x0 0x0                        CapstoneCore.Capstone+cs_detail
0x8 [2] xor edi, esp ; 0x31 0xe7 0x0 0x0                        CapstoneCore.Capstone+cs_detail
0xA [6] fsub qword ptr [rcx + 0x4ee8f32e] ; 0xdc 0xa1 0x2e 0xf3 CapstoneCore.Capstone+cs_detail
0x10 [1] .byte 0x62 ; 0x62 0x0 0x0 0x0                          CapstoneCore.Capstone+cs_detail
0x11 [1] .byte 0xf3 ; 0xf3 0x0 0x0 0x0                          CapstoneCore.Capstone+cs_detail
```
