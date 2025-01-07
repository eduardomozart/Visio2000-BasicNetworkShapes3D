# Visio2000-BasicNetworkShapes3D
 Basic Network Shapes 3D stencils from Visio 2000 to PlantUML sprites.

 The VSS stencil to SVG/PNG conversion process has been documented [here](https://translate.google.com/translate?sl=pt&tl=en&hl=pt-BR&u=https://eduardomozartdeoliveira.wordpress.com/2023/01/30/instalacao-do-libvisio2svg-no-macos/).

 ## Samples

![Sample](Sample.png)

### Network Diagram

![Basic Usage - Network Diagram](https://www.plantuml.com/plantuml/png/nLDTJy8m57tlhxWItenh0NrPa23mY8H892REcBeMrh3TBcqdKSD_j_juy0EZ3ufBjfsiP-VSUtfBXjPnuuei9UH8o9L22KjbbUvkPj91ubnkGqeDtmPhvPBYeR3In1gTH1V4EgDI5Dm8dUbdBqFhNnbZ9oDkLUmbjjfi5WdFfUrDQCOLaYE5SLg8jpuqzmNGXJIFqWGb_feqbyPgvEczDyyBzor_odEdyvf4-jOzfN90S2iKNq_yRNW6BmJ0LjuL11ZnUBCska0nrgasW1fbjJ3ryNpuv1yxiYDzsaWtsfNIoh8Et0ffOwDofpJ2ERJwryUCTTdWtzxjEkT1X2LGGfiG5bTBrebmplqqG9bi026Cm-YIOy6LZN3CCuM93Y7oLyrkrbftnBUAzKx3z6BMX5Ytty0uLNvWzgNH_hIXlZ0OLtpfqK_RkWbz8U_CkdlCwcduBOVU8TivFQJPsP-RbOTcA56Kv_8L)

```csharp
@startuml

!define Visio2kNet https://raw.githubusercontent.com/eduardomozart/Visio2000-BasicNetworkShapes3D/main
!include Visio2kNet/puml/Server.puml
!include Visio2kNet/puml/Personal_computer.puml
!include Visio2kNet/puml/Laptop.puml

<style>
nwdiagDiagram {
  server {
    BackgroundColor none
    LineColor none
    
  }
}
</style>

nwdiag {
  fs01 [description = "<U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><$Server>\nServidor: SRV01\nPasta comp. : C:\Manuais\nCaminho: \\\\SRV01\Manuais"]

  network LAN {
      fs01
      client01 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client02 [description = "<$Laptop>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client03 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client04 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client05 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
  }
}
@enduml
```